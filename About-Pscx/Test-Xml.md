---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Test-Xml

## SYNOPSIS
PSCX Cmdlet: Tests for well formedness and optionally validates against XML Schema.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Test-Xml [-Path] <String[]> [-EnableDtd] [-SchemaPath <String[]>] [-Validate] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Test-Xml -InputObject <PSObject> [-EnableDtd] [-SchemaPath <String[]>] [-Validate] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Test-Xml [-LiteralPath] <String[]> [-EnableDtd] [-SchemaPath <String[]>] [-Validate] [<CommonParameters>]
```

## DESCRIPTION
Tests for well formedness and optionally validates against XML Schema. 
It doesn't handle specifying the targetNamespace. 
To see validation error messages, specify the -Verbose flag.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\PS> Test-Xml foo.xml
```

Returns true or false indicating whether or not foo.xml is well-formed.

### EXAMPLE 2
PS C:\\\>

```
C:\PS> Test-Xml foo.xml -Verbose
```

Returns true or false indicating whether or not foo.xml is well-formed and displays any XML error info.

### EXAMPLE 3
PS C:\\\>

```
C:\PS> Test-Xml foo.xml -SchemaPath .\foo.xsd
```

Returns true or false indicating whether or not foo.xml is well-formed and conforms to the schema defined in foo.xsd.

### EXAMPLE 4
PS C:\\\>

```
C:\PS> Test-Xml foo.xml -EnableDtd
```

Returns true or false indicating whether or not foo.xml is well-formed.
This examples enables DTD processing for XML files that use a DTD.

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

### -SchemaPath
Array of paths to the required schema files to perform schema-based validation.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Validate
Forces schema validation of the XML against inline schema.

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

[Format-Xml]()

