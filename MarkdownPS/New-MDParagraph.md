---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDParagraph

## SYNOPSIS
This commandlet output paragraph in markdown syntax

## SYNTAX

```
New-MDParagraph [[-Lines] <String[]>] [-NoNewLine] [<CommonParameters>]
```

## DESCRIPTION
This commandlet output paragraph in markdown syntax

## EXAMPLES

### EXAMPLE 1
```
New-MDParagraph
```

An empty line

### EXAMPLE 2
```
New-MDParagraph -Lines "Line 1"
"Line 1" | New-MDParagraph
```

Line 1

### EXAMPLE 3
```
New-MDParagraph -Lines @("Line 1","Line 2")
@("Line 1","Line 2") | New-MDParagraph
```

Line 1
Line 2

## PARAMETERS

### -Lines
An array of lines to paragraph in markdown

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
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

### Each line
## NOTES
Use the -NoNewLine parameter when you don't want the next markdown content to be separated.

## RELATED LINKS

[New-MDHeader
https://help.github.com/articles/basic-writing-and-formatting-syntax/]()

