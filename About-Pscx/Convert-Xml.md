---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Convert-Xml

## SYNOPSIS
PSCX Cmdlet: Performs XSLT transforms on the specified XML file or XmlDocument.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Convert-Xml [-Path] <String[]> [-XsltPath] <String> [-ConformanceLevel <ConformanceLevel>]
 [-EnableDocumentFunction] [-EnableDtd] [-EnableScript] [-OutputPath <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Convert-Xml [-XsltPath] <String> -InputObject <PSObject> [-ConformanceLevel <ConformanceLevel>]
 [-EnableDocumentFunction] [-EnableDtd] [-EnableScript] [-OutputPath <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Convert-Xml [-LiteralPath] <String[]> [-XsltPath] <String> [-ConformanceLevel <ConformanceLevel>]
 [-EnableDocumentFunction] [-EnableDtd] [-EnableScript] [-OutputPath <String>] [<CommonParameters>]
```

## DESCRIPTION
Performs XSLT transforms on the specified XML file or XmlDocument. 
Use the EnableScript parameter to enable script embedded in the XSLT file.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\PS> Convert-Xml foo.xml foo.xslt
```

Transforms the XML in the input file foo.xml based on the XSLT specified foo.xslt.

### EXAMPLE 2
PS C:\\\>

```
C:\PS> Convert-Xml foo.xml bar.xslt -EnableScript
```

Transforms the XML in the input file foo.xml based on the XSLT specified foo.xslt while enabling embedded script to be processed.

## PARAMETERS

### -LiteralPath
Specifies a path to the item.
The value of -LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell Windows PowerShell not to interpret any characters as escape sequences.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Specifies the path to the file to process.
Wildcard syntax is allowed.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -XsltPath
Path to the XSLT file to apply during the transform.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Accepts an object as input to the cmdlet.
Enter a variable that contains the objects or type a command or expression that gets the objects.

```yaml
Type: PSObject
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ConformanceLevel
@{Text=}

```yaml
Type: ConformanceLevel
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableDocumentFunction
Enable the document() function in XPath expressions.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableDtd
Enables document type definition (DTD) processing.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableScript
Enable embedded script blocks in the XSLT.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputPath
If set, specifies the path to a file to receive the output.
No characters are interpreted as wildcards.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS

[Test-Xml]()

[Format-Xml]()

