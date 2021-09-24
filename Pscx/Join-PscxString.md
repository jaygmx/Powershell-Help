---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Join-PscxString

## SYNOPSIS
PSCX Cmdlet: Joins an array of strings into a single string.

## SYNTAX

### NewLineSeparator (Default)
```
Join-PscxString [-Strings] <String[]> [-NewLine] [<CommonParameters>]
```

### CustomSeparator
```
Join-PscxString [-Strings] <String[]> [-Separator <String>] [<CommonParameters>]
```

## DESCRIPTION
Joins an array of strings into a single string.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Strings
String(s) to be joined.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NewLine
Insert newline as separator between joined strings.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: NewLineSeparator
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Separator
Insert specified string as the separator between joined strings.

```yaml
Type: System.String
Parameter Sets: CustomSeparator
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

[Split-String]()

