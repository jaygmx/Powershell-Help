---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Format-Xml

## SYNOPSIS
PSCX Cmdlet: Pretty print for XML files and XmlDocument objects.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Format-Xml [-Path] <String[]> [-AttributesOnNewLine] [-ConformanceLevel <ConformanceLevel>] [-EnableDtd]
 [-IndentString <String>] [-OmitXmlDeclaration] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Format-Xml -InputObject <PSObject> [-AttributesOnNewLine] [-ConformanceLevel <ConformanceLevel>] [-EnableDtd]
 [-IndentString <String>] [-OmitXmlDeclaration] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Format-Xml [-LiteralPath] <String[]> [-AttributesOnNewLine] [-ConformanceLevel <ConformanceLevel>] [-EnableDtd]
 [-IndentString <String>] [-OmitXmlDeclaration] [<CommonParameters>]
```

## DESCRIPTION
Pretty print for XML files and XmlDocument objects.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\PS> Format-Xml foo.xml
```

Formats the XML in foo.xml in a "pretty print" manner.

### EXAMPLE 2
PS C:\\\>

```
C:\PS> Format-Xml foo.xml -AttributesOnNewLine
```

Formats the XML in foo.xml in a "pretty print" manner putting each attribute on a new line.

### EXAMPLE 3
PS C:\\\>

```
C:\PS> Format-Xml foo.xml -EnableDtd
```

Formats the XML in foo.xml which uses a DTD in a "pretty print" manner.

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

### -AttributesOnNewLine
Write attributes on a new line.

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

### -ConformanceLevel
Conformance level for XML.

```yaml
Type: ConformanceLevel
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Auto
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

### -IndentString
The string to use for indenting.

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

### -OmitXmlDeclaration
Omit the XML declaration element.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS

[Convert-Xml]()

[Test-Xml]()

