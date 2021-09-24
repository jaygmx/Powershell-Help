---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDQuote

## SYNOPSIS
This commandlet output quote in markdown syntax

## SYNTAX

```
New-MDQuote [-Lines] <String[]> [-Level <Int32>] [-NoNewLine] [<CommonParameters>]
```

## DESCRIPTION
This commandlet output quote in markdown syntax by adding a '\> ' in front of each line

## EXAMPLES

### EXAMPLE 1
```
New-MDQuote -Lines "Line 1"
```

\> Line 1

### EXAMPLE 2
```
New-MDQuote -Lines @("Line 1","Line 2")
```

\> Line 1
\> 
\> Line 2

### EXAMPLE 3
```
@("Line 1","Line 2") | New-MDQuote -Level 2
```

\>\> Line 1
\>\>
\>\> Line 2

## PARAMETERS

### -Lines
An array of lines to quote in markdown

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
The level of quote

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

### Each line with a '> ' in the front
## NOTES
Use the -NoNewLine parameter when you don't want the next markdown content to be separated.

## RELATED LINKS

[New-MDCode
https://help.github.com/articles/basic-writing-and-formatting-syntax/]()

