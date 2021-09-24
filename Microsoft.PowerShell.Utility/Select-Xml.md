---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
Module Name: Microsoft.PowerShell.Utility
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/select-xml?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Select-Xml

## SYNOPSIS
Finds text in an XML string or document.

## SYNTAX

### Xml (Default)
```
Select-Xml [-Xml] <XmlNode[]> [-XPath] <String> [-Namespace <Hashtable>] [<CommonParameters>]
```

### Path
```
Select-Xml [-Path] <String[]> [-XPath] <String> [-Namespace <Hashtable>] [<CommonParameters>]
```

### LiteralPath
```
Select-Xml -LiteralPath <String[]> [-XPath] <String> [-Namespace <Hashtable>] [<CommonParameters>]
```

### Content
```
Select-Xml -Content <String[]> [-XPath] <String> [-Namespace <Hashtable>] [<CommonParameters>]
```

## DESCRIPTION
The \`Select-Xml\` cmdlet lets you use XPath queries to search for text in XML strings and documents.
Enter an XPath query, and use the Content , Path , or Xml parameter to specify the XML to be searched.

## EXAMPLES

### Example 1: Select AliasProperty nodes
```
$Path = "$Pshome\Types.ps1xml"
$XPath = "/Types/Type/Members/AliasProperty"
Select-Xml -Path $Path -XPath $Xpath | Select-Object -ExpandProperty Node

Name                 ReferencedMemberName
----                 --------------------
Count                Length
Name                 Key
Name                 ServiceName
RequiredServices     ServicesDependedOn
ProcessName          Name
Handles              Handlecount
VM                   VirtualSize
WS                   WorkingSetSize
Name                 ProcessName
Handles              Handlecount
VM                   VirtualMemorySize
WS                   WorkingSet
PM                   PagedMemorySize
NPM                  NonpagedSystemMemorySize
Name                 __Class
Namespace            ModuleName
```

The result shows the Name and ReferencedMemberName of each alias property in the \`Types.ps1xml\` file.
For example, there is a Count property that is an alias of the Length property.

### Example 2: Input an XML document
```
[xml]$Types = Get-Content $Pshome\Types.ps1xml
Select-Xml -Xml $Types -XPath "//MethodName"
```

### Example 3: Search PowerShell Help files
```
$Namespace = @{
    command = "http://schemas.microsoft.com/maml/dev/command/2004/10"
    maml = "http://schemas.microsoft.com/maml/2004/10"
    dev = "http://schemas.microsoft.com/maml/dev/2004/10"
}

$Path = "$Pshome\en-us\*dll-Help.xml"
$Xml = Select-Xml -Path $Path -Namespace $Namespace -XPath "//command:name"
$Xml | Format-Table @{Label="Name"; Expression= {($_.node.innerxml).trim()}}, Path -AutoSize

Name                    Path
----                    ----
Export-Counter          C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Diagnostics.dll-Help.xml
Get-Counter             C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Diagnostics.dll-Help.xml
Get-WinEvent            C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Diagnostics.dll-Help.xml
Import-Counter          C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Diagnostics.dll-Help.xml
Add-Computer            C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Management.dll-Help.xml
Add-Content             C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Management.dll-Help.xml
Checkpoint-Computer     C:\Windows\system32\WindowsPowerShell\v1.0\en-us\Microsoft.PowerShell.Commands.Management.dll-Help.xml
...
```

### Example 4: Different ways to input XML
```
$Xml = @"
<?xml version="1.0" encoding="utf-8"?>
<Book>
  <projects>
    <project name="Book1" date="2009-01-20">
      <editions>
        <edition language="English">En.Book1.com</edition>
        <edition language="German">Ge.Book1.Com</edition>
        <edition language="French">Fr.Book1.com</edition>
        <edition language="Polish">Pl.Book1.com</edition>
      </editions>
    </project>
  </projects>
</Book>
"@

Select-Xml -Content $Xml -XPath "//edition" | foreach {$_.node.InnerXML}

En.Book1.com
Ge.Book1.Com
Fr.Book1.com
Pl.Book1.com

$Xml | Select-Xml -XPath "//edition" | foreach {$_.node.InnerXML}

En.Book1.com
Ge.Book1.Com
Fr.Book1.com
Pl.Book1.com
```

### Example 5: Use the default xmlns namespace
```
$SnippetNamespace = @{snip = "http://schemas.microsoft.com/PowerShell/Snippets"}

Select-Xml -Path $Home\Documents\WindowsPowerShell\Snippets -Namespace $SnippetNamespace -XPath "//snip:Title" |
    ForEach-Object {$_.Node.Innerxml}
```

## PARAMETERS

### -Content
Specifies a string that contains the XML to search.
You can also pipe strings to \`Select-Xml\`.

```yaml
Type: System.String[]
Parameter Sets: Content
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LiteralPath
Specifies the paths and file names of the XML files to search.
Unlike Path , the value of the LiteralPath parameter is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell PowerShell not to interpret any characters as escape sequences.

```yaml
Type: System.String[]
Parameter Sets: LiteralPath
Aliases: PSPath, LP

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Namespace
Specifies a hash table of the namespaces used in the XML.
Use the format\`@{\<namespaceName\> = \<namespaceValue\>}\`.

When the XML uses the default namespace, which begins with xmlns, use an arbitrary key for the namespace name.
You cannot use xmlns.
In the XPath statement, prefix each node name with the namespace name and a colon, such as \`//namespaceName:Node\`.

```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
Specifies the path and file names of the XML files to search.
Wildcard characters are permitted.

```yaml
Type: System.String[]
Parameter Sets: Path
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Xml
Specifies one or more XML nodes.

An XML document will be processed as a collection of XML nodes.
If you pipe an XML document to \`Select-Xml\`, each document node will be searched separately as it comes through the pipeline.

```yaml
Type: System.Xml.XmlNode[]
Parameter Sets: Xml
Aliases: Node

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -XPath
Specifies an XPath search query.
The query language is case-sensitive.
This parameter is required.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String or System.Xml.XmlNode
You can pipe a path or XML node to this cmdlet.

## OUTPUTS

### Microsoft.PowerShell.Commands.SelectXmlInfo
## NOTES
XPath is a standard language that is designed to identify parts of an XML document.
For more information about the XPath language, see XPath Reference (/dotnet/standard/data/xml/select-nodes-using-xpath-navigation)and the Selection Filters section of Event Selection (/previous-versions//aa385231(v=vs.85)).

## RELATED LINKS

[ConvertTo-Xml]()

