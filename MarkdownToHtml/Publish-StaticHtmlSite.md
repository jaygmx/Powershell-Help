---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/Publish-StaticHtmlSite.html
schema: 2.0.0
---

# Publish-StaticHtmlSite

## SYNOPSIS
Create a static HTML site from HTML fragment objects.

## SYNTAX

```
Publish-StaticHtmlSite [-InputObject] <Object> [[-Template] <String>] [[-ContentMap] <Hashtable>]
 [[-MediaDirectory] <String>] [-SiteDirectory] <String> [<CommonParameters>]
```

## DESCRIPTION
Html fragment objects piped into this function (or passed via the \`InputObject\`
parameter) are converted into standalone HTML documents and saved to a Html site
directory.

The Markdown to HTML document conversion uses default or custom templates with
stylesheets and JavaScript resources to render Markdown extensions for:
* LaTeX math
* code syntax highlighting
* diagrams

See \`New-HtmlTemplate\` for details.

## EXAMPLES

### EXAMPLE 1
```
Find-MarkdownFiles '...\Modules\MarkdownToHtml' | Convert-MarkdownToHTMLFragment | Publish-StaticHtmlSite -SiteDirectory 'e:\temp\site'
```

Generates a static HTML site from the Markdown files in '...\Modules\MarkdownToHtml'.
This is
a simpler version of the functionality provided by the function \`Convert-MarkdownToHTML\`.

The generated Html file objects are returned like so:

    Mode                LastWriteTime         Length Name
    ----                -------------         ------ ----
    -a----       15.09.2019     10:03          16395 Convert-MarkdownToHTML.html
    -a----       15.09.2019     10:03          14714 Convert-MarkdownToHTMLFragment.html
    -a----       15.09.2019     10:03           4612 Find-MarkdownFiles.html
    -a----       15.09.2019     10:03           6068 MarkdownToHTML.html
    ... 
... 
... 
...

## PARAMETERS

### -InputObject
An object representing an Html fragment.
Ideally this is an output object
returned by \`Convert-MarkdownToHTMLFragment\`, but any object will
work provided following properties are present:

\`RelativePath\`
:   A string representing the relative path to the Markdown file with respect to
    a base (static site) directory.
    This property is automatically provided by:
    * using the PowerShell function \`Find-MarkdownFiles\`
    * piping a file object \`\[System.IO.FileInfo\]\` into
      \`Convert-MarkdownToHTMLFragment\` (or passing it as a parameter).

\`Title\`
:   The page title.

\`HtmlFragment\`
:   A html fragment, as string or array of strings to be used as main content of
    the HTML document.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases: HtmlFragment

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Template
Optional directory containing the html template file \`md-template.html\` and its
resources which will be used to convert the Html fragments into standalone Html
documents.
If no template directory is specified, a default factory-installed
template is used.
For infomations about creating custom templates see
\`New-HTMLTemplate\`.
See
\[Template Customization\](about_MarkdownToHTML.md#conversion-template-customization)
for customization options.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: (Join-Path $SCRIPT:moduleDir.FullName 'Template')
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContentMap
Placeholder substitution mapping as described in
\[Template Customization\](about_MarkdownToHTML.md#conversion-template-customization).

Following substitution mappings are used by default unless explicitely defined.

| Placeholder   | Description                  | Origin                      |
|:------------- | :--------------------------- | :-------------------------- |
| \`{{title}}\`   | Auto generated page title    | \`$inputObject.Title\`        |
| \`\[title\]\`     | For backwards compatibility.
| \`$inputObject.Title\`        |
| \`{{content}}\` | HTML content                 | \`$inputObject.HtmlFragment\` |
| \`\[content\]\`   | For backwards compatibility.
| \`$inputObject.HtmlFragment\` |

For static HTML site projects additional mappings are defined:

| Placeholder   | Description                  | Origin       |
|:------------- | :--------------------------- | :----------- |
| \`{{nav}}\`     | Navigation bar content       | \`Build.json\` |
| \`{{footer}}\`  | Page footer content          | \`Build.json\` |

For static HTML site projects additional placeholders can be added to the map.
See
\[Defining Content Mapping Rules\](about_MarkdownToHTML.md#defining-content-mapping-rules)

```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MediaDirectory
An optional directory containing additional media for the HTML site
such as images, videos etc.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteDirectory
Directory for the generated HTML files.
The Html files will be placed
in the same relative location below this directory as related Markdown document
has below the input directory.
If the site directory does not exist it will be created.
If the site directory already exists its files will be retained, but possibly overwitten
by generated HTML files.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### An Html Fragment objects having the properties `RelativePath`,`Title`, `HtmlFragment` , and
### optionally `ContentMap`. See the description of the `InputObject` parameter for details
## OUTPUTS

### File objects [System.IO.FileInfo] of the generated HTML documents.
## NOTES

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/Publish-StaticHtmlSite.html](https://wethat.github.io/MarkdownToHtml/2.5.0/Publish-StaticHtmlSite.html)

[`Convert-MarkdownToHTML`]()

[`Find-MarkdownFiles`]()

[`Convert-MarkdownToHTMLFragment`]()

[`New-HTMLTemplate`]()

[[Defining Content Mapping Rules](about_MarkdownToHTML.md#defining-content-mapping-rules)]()

