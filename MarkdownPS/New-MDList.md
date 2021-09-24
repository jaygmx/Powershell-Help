---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDList

## SYNOPSIS
This commandlet output list in markdown syntax

## SYNTAX

```
New-MDList [-Lines] <String[]> [-Level <Int32>] -Style <String> [-NoNewLine] [<CommonParameters>]
```

## DESCRIPTION
This commandlet output list in markdown syntax.
Depending if the list is unordered or ordere, the '- ' or '1.
' is added in front of each line

## EXAMPLES

### EXAMPLE 1
```
New-MDList -Lines "Line 1" -Style Unordered
"Line 1" | New-MDList -Style Unordered
```

- Line 1

### EXAMPLE 2
```
New-MDList -Lines @("Line 1","Line 2") -Style Unordered
@("Line 1","Line 2") | New-MDList -Style Unordered
```

- Line 1
- Line 2

### EXAMPLE 3
```
New-MDList -Lines "Line 1" -Style Ordered
"Line 1" | New-MDList -Style Ordered
```

1.
Line 1

### EXAMPLE 4
```
New-MDList -Lines @("Line 1","Line 2") -Style Ordered
@("Line 1","Line 2") | New-MDList -Style Ordered
```

1.
Line 1
2.
Line 2

## PARAMETERS

### -Lines
An array of lines to make a list in markdown

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

### -Level
The level of list

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 1
Accept pipeline input: False
Accept wildcard characters: False
```

### -Style
The type of list.
Ordered or Unordered

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoNewLine
Controls if a new line is added at the end of the output

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### An array of lines
## OUTPUTS

### Each line with a '- ' or '1. ' in the front depending on the type of the list.
## NOTES
Use the -NoNewLine parameter when you don't want the next markdown content to be separated.

## RELATED LINKS

[New-MDParagraph
https://help.github.com/articles/basic-writing-and-formatting-syntax/]()

