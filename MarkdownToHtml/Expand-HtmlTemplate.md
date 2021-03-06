---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/Expand-HtmlTemplate.html
schema: 2.0.0
---

# Expand-HtmlTemplate

## SYNOPSIS
Simple template expansion based on a content substitution dictionary.

## SYNTAX

```
Expand-HtmlTemplate [-InputObject] <String> [-ContentMap] <Hashtable> [<CommonParameters>]
```

## DESCRIPTION
Locates placeholders in the input string abd replaced them
with values found for the placeholders in the given dictionary.
The placeholder
expansion is non-recursive.

## EXAMPLES

### EXAMPLE 1
```
Expand-HtmlTemplate -InputObject $template -ContentMap $map
```

Expand the HTML template \`$template\` mappings provided with \`$map\`.

With:

~~~ PowerShell
$template = '\<span class="navitem{{level}}"\>{{navtext}}\</span\>'
$map = @{
    '{{level}}'   = 1
    '{{navtext}}' = 'foo'
}
~~~

this HTML fragment is generated:

~~~ html
\<span class="navitem1"\>foo\</span\>
~~~

## PARAMETERS

### -InputObject
An string representing an Html fragment.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Template

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ContentMap
A dictionary whose keys define placeholders and whose values define the
replacements.

```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### HTML template with placeholders.
## OUTPUTS

### HTML fragment with all paceholders replaced by the content specified
### by the `ContentMap`.
## NOTES

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/Expand-HtmlTemplate.html](https://wethat.github.io/MarkdownToHtml/2.5.0/Expand-HtmlTemplate.html)

