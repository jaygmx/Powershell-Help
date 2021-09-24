---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDLink

## SYNOPSIS
This commandlet output link in markdown syntax

## SYNTAX

```
New-MDLink [-Text] <String> -Link <String> [-Title <String>] [<CommonParameters>]
```

## DESCRIPTION
This commandlet output link in markdown syntax like this \[text\](link "title")

## EXAMPLES

### EXAMPLE 1
```
New-MDLink -Text "Example" -Link "http://example.com"
"example.png" | New-MDLink -Link "http://example.com"
```

\[Example\](http://example.com)

### EXAMPLE 2
```
New-MDLink -Text "Example" -Link "http://example.com" -Title "This is an example link"
"example.png" | New-MDLink -Link "http://example.com" -Title "This is an example link"
```

\[Example\](http://example.com "This is an example link")

## PARAMETERS

### -Text
Text of the link

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

### -Link
The link

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

### -Title
The title of the link

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

### Any text
## OUTPUTS

### The link construct in markdown
## NOTES

## RELATED LINKS

[New-MDImage
https://help.github.com/articles/basic-writing-and-formatting-syntax/]()

