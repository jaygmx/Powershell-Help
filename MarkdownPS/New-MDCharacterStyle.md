---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDCharacterStyle

## SYNOPSIS
This commandlet output bold, italic or strikethrough in markdown syntax

## SYNTAX

```
New-MDCharacterStyle [-Text] <String> -Style <String> [<CommonParameters>]
```

## DESCRIPTION
This commandlet output bold, italic or strikethrough in markdown syntax by wrapping the text in **, * or ~~ respectively.

## EXAMPLES

### EXAMPLE 1
```
New-MDCharacterStyle -Text "Bold" -Style "Bold"
"Bold" | New-MDCharacterStyle -Style "Bold"
```

**Bold**

### EXAMPLE 2
```
New-MDCharacterStyle -Text "Italic" -Style "Italic"
"Italic" | New-MDCharacterStyle -Style "Italic"
```

*Italic*

### EXAMPLE 3
```
New-MDCharacterStyle -Text "StrikeThrough" -Style "StrikeThrough"
"StrikeThrough" | New-MDCharacterStyle -Style "StrikeThrough"
```

~~StrikeThrough~~

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

### -Style
One of the Bold, Italic or StrikeThrough

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Any text
## OUTPUTS

### The input wrapped in **, * or ~~ respectively for bold, italic or strikethrough
## NOTES

## RELATED LINKS

[New-MDInlineCode]()

