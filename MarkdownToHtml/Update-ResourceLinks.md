---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/Update-ResourceLinks.html
schema: 2.0.0
---

# Update-ResourceLinks

## SYNOPSIS
Rewrite resource links which are relative to the projects root to make them
valid for other site locations.

## SYNTAX

```
Update-ResourceLinks [-InputObject] <String> [[-RelativePath] <String>] [<CommonParameters>]
```

## DESCRIPTION
HTML templates use links which are relative to the HTML site root directory
to link to resources such as JavaScript, css, or image files.
When a HTML
file is assembled (e.g with \`\`Publish-StaticHtmlSite\`\`) using such a template,
the resource links in the template may not be valid for the location of that
HTML file.
This command uses the relative position of the new HTML file in the
site to compute valid resource links and update the template.

## EXAMPLES

### EXAMPLE 1
```
Update-ResourceLinks -HtmlFragment $fragment -RelativePath 'a/b/v/test.html'
```

Adjust link to a resource at \`images/logo.png\` so that it is valid for a
file located at \`a/b/v/test.html\`.
The input \`$fragment\` is defined as:

~~~ PowerShell
$fragment = '\<img width="90%" src="images/logo.png"/\>'
~~~

Outut:

~~~ html
\<img width="90%" src="../../../images/logo.png"/\>
~~~

## PARAMETERS

### -InputObject
An html fragment containing root-relative resource links.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: HtmlFragment

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -RelativePath
The path to a Markdown (\`*.md\`) or HTML (\`*.html\`) file relative to its root
directory.
That file's relative path
is used to adjust the links of in the given navigation bar item,
so that it can be reached from the location of the HTML page currently being
assembled.

The given path should use forward slash '/' path separators.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### HTML fragments containing resource links relative to the HTML site root.
## OUTPUTS

### HTML fragment with updated resource links.
## NOTES

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/Update-ResourceLinks.html](https://wethat.github.io/MarkdownToHtml/2.5.0/Update-ResourceLinks.html)

[`Publish-StaticHtmlSite`]()

