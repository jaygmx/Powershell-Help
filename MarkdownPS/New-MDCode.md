---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDCode

## SYNOPSIS
This commandlet output code block in markdown syntax

## SYNTAX

```
New-MDCode [-Lines] <String[]> [-Style <String>] [<CommonParameters>]
```

## DESCRIPTION
This commandlet output code blocke in markdown syntax by wrapping around \`\`\`

## EXAMPLES

### EXAMPLE 1
```
New-MDCode -Lines "Line 1"
"Line 1" | New-MDCode
```

\`\`\`
    Line 1
\`\`\`

### EXAMPLE 2
```
New-MDCode -Lines @("Line 1","Line 2")
@("Line 1","Line 2") | New-MDCode
```

\`\`\`
    Line 1
    Line 2
\`\`\`

### EXAMPLE 3
```
New-MDCode -Lines @("Line 1","Line 2") -Style "powershell"
@("Line 1","Line 2") | New-MDCode -Style "powershell"
```

\`\`\`powershell
    Line 1
    Line 2
\`\`\`

## PARAMETERS

### -Lines
An array of lines to code block in markdown

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

### -Style
The style of code.
e.g.
powershell or xml or javascript

```yaml
Type: System.String
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

### An array of lines
## OUTPUTS

### Input wrapped in ```
## NOTES

## RELATED LINKS

[New-MDQuote
https://help.github.com/articles/basic-writing-and-formatting-syntax/]()

