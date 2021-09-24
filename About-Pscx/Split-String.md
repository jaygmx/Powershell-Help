---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Split-String

## SYNOPSIS
PSCX Cmdlet: Splits a single string into an array of strings.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Split-String [-Input] <String> [[-Separator] <String[]>] [-Count <Int32>] [-NewLine] [-RemoveEmptyStrings]
 [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Split-String [-Input] <String> [-CaseSensitive] [-Count <Int32>] [-MultiLine] [-RegexSeparator <String>]
 [-RemoveEmptyStrings] [-SingleLine] [<CommonParameters>]
```

## DESCRIPTION
Splits a single string into an array of strings.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Input
String input to be split.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Separator
Array of characters or string to use for separator. 
Null value or empty array will result in white space being used as separator.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CaseSensitive
Indicates that the regex is case sensitive.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Count
Maximum count of substrings to output.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MultiLine
Enables the Multiline regex option.
^ and $ will match begging and end of each line in a single string.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NewLine
Add environment's newline string as a separator.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RegexSeparator
Regular expression pattern to use as a separator.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveEmptyStrings
If specified, empty substrings will be removed from output.

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

### -SingleLine
Enables the Singeline regex option.
The period character (.) will match every character including newline characters.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

[Join-PscxString]()

