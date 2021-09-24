---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Test-AlternateDataStream

## SYNOPSIS
PSCX Cmdlet: Tests for the existence of the specified alternate data stream from an NTFS file.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Test-AlternateDataStream [-Path] <String[]> [-Name] <String> [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Test-AlternateDataStream [-LiteralPath] <String[]> [-Name] <String> [<CommonParameters>]
```

## DESCRIPTION
Tests for the existence of the specified alternate data stream from an NTFS file.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\PS> Get-ChildItem *.zip | Test-AlternateDataStream -Name Zone.Identifier -Verbose
```

Shows which ZIP files have an alternate data stream named Zone.Identifier.

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

### -Name
Specifies the name of the alternate data stream e.g.
Zone.Identifier

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS
