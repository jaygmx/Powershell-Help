---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDInlineCode

## SYNOPSIS
This commandlet output inline code in markdown syntax

## SYNTAX

```
New-MDInlineCode [-Text] <String> [<CommonParameters>]
```

## DESCRIPTION
This commandlet output inline code in markdown syntax by wrapping the text in \`

## EXAMPLES

### EXAMPLE 1
```
New-MDInlineCode -Text "Inline Code"
"Inline Code" | New-MDInlineCode
```

\`Inline Code\`

## PARAMETERS

### -Text
Any text

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Any text
## OUTPUTS

### The input wrapped in `
## NOTES

## RELATED LINKS

[New-MDQuote
New-MDCharacterStyle
https://help.github.com/articles/basic-writing-and-formatting-syntax/]()

