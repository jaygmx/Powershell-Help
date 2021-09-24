---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Test-Xml

## SYNOPSIS
PSCX Cmdlet: Tests for well formedness and optionally validates against XML Schema.

## SYNTAX

### Path (Default)
```
Test-Xml [-SchemaPath <PscxPathInfo[]>] [-Validate] [-EnableDtd] [-Path] <PscxPathInfo[]> [<CommonParameters>]
```

### Object
```
Test-Xml [-SchemaPath <PscxPathInfo[]>] [-Validate] [-EnableDtd] -InputObject <PSObject> [<CommonParameters>]
```

### LiteralPath
```
Test-Xml [-SchemaPath <PscxPathInfo[]>] [-Validate] [-EnableDtd] [-LiteralPath] <PscxPathInfo[]>
 [<CommonParameters>]
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
Type: Pscx.IO.PscxPathInfo[]
Parameter Sets: LiteralPath
Aliases: PSPath

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
Type: Pscx.IO.PscxPathInfo[]
Parameter Sets: Path
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
Type: System.Management.Automation.PSObject
Parameter Sets: Object
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
Type: System.Management.Automation.SwitchParameter
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
Type: Pscx.IO.PscxPathInfo[]
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
Type: System.Management.Automation.SwitchParameter
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

## RELATED LINKS

[Convert-Xml]()

[Format-Xml]()

