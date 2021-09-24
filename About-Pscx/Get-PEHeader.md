---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-PEHeader

## SYNOPSIS
PSCX Cmdlet: Gets the Portable Header information from an executable file.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-PEHeader [-Path] <String[]> [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-PEHeader [-LiteralPath] <String[]> [<CommonParameters>]
```

## DESCRIPTION
The PE header for Windows executables includes various useful bits of information including the image base address, subsystem, linker version, etc.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
Get-PEHeader $PSHome\PowerShell.exe
```

## PARAMETERS

### -LiteralPath
Specifies a path to the item.
The value of -LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell Windows PowerShell not to interpret any characters as escape sequences.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_2
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
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS
