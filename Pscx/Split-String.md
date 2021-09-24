---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Split-String

## SYNOPSIS
PSCX Cmdlet: Splits a single string into an array of strings.

## SYNTAX

### StringSeparator (Default)
```
Split-String [[-Separator] <String[]>] [-Input] <String> [-NewLine] [-RemoveEmptyStrings] [-Count <Int32>]
 [<CommonParameters>]
```

### RegularExpressionSeparator
```
Split-String [-Input] <String> [-RegexSeparator <String>] [-CaseSensitive] [-MultiLine] [-SingleLine]
 [-RemoveEmptyStrings] [-Count <Int32>] [<CommonParameters>]
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
Type: System.String
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
Type: System.String[]
Parameter Sets: StringSeparator
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: RegularExpressionSeparator
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
Type: System.Int32
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: RegularExpressionSeparator
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: StringSeparator
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
Type: System.String
Parameter Sets: RegularExpressionSeparator
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
Type: System.Management.Automation.SwitchParameter
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: RegularExpressionSeparator
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

[Join-PscxString]()

