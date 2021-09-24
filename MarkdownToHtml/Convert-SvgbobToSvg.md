---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/Convert-SvgbobToSvg.html
schema: 2.0.0
---

# Convert-SvgbobToSvg

## SYNOPSIS
Convert fenced svgbob code blocks to svg images.

## SYNTAX

```
Convert-SvgbobToSvg [-InputObject] <Hashtable> [-SiteDirectory] <String> [[-Options] <Object>]
 [<CommonParameters>]
```

## DESCRIPTION
Scans the input data (lines of Markdown text) for svgbob fenced code blocks
and converts them to a Markdown style image link to a svg file containing
the rendered diagram.

Svgbob code blocks define human readable diagrams and are labeled as \`bob\`.
For example:

\`\`\` Markdown
~~~ bob
      +------+   .-. 
+---+
 o----| elem |--( ; )--| n |----o
      +------+   '-'   +---+
~~~
\`\`\`

The generated svg file is put right next to the HTML file
currently being assembled and named after that HTML file with an unique
index appended.

## EXAMPLES

### EXAMPLE 1
```
Convert-MarkdownToHTMLFragment -InputObject $md -Split | Convert-SvgbobToSvg -SiteDirectory $site -RelativePath $relativePath
```

Read Markdown content from the file \`$md\` and replace all fenced code blocks
marled as \`bob\` with Markdown style image links to the svg version of the
diagram.
The conversion is performed using default svg rendering options.

Where

\`$site\`
:   Is the **absolute path** to the HTML site's root directory

\`$relativePath\`
:   is the **relative path** of the HTML file currently being assembled below
    \`$site\`.

\`$md\`
:   is a Markdown file \`test.md\` which contains a fenced svgbob diagram:
    \`\`\` Markdown
    Some text ...

    ~~~ bob
          +------+   .-. 
+---+
     o----| elem |--( ; )--| n |----o
          +------+   '-'   +---+
    ~~~

    Some more text ...
    \`\`\`

this fragment is converted to:

* A file \`test1.svg\` which is placed right next to the html file \`test.html\`
  which is going to be created by \`Publish-StaticHtmlSite\` in a subsequent
  stage of the conversion pipeline.
The numerical postfix is the index of the
  Svgbob diagram in the fragment.
The svg image renders as:

  ~~~ bob
       +------+   .-. 
+---+
  o----| elem |--( ; )--| n |----o
       +------+   '-'   +---+
  ~~~

* An updated html fragment where the fenced Svgbob diagram is replaced with
  a reference to the svg image.

  ~~~ html
  Some text ...

  \<img src='test1.svg' alt='Diagram 1.' /\>

  Some more text ...
  ~~~

## PARAMETERS

### -InputObject


```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases: HtmlFragment

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SiteDirectory
Location of the static HTML site.
The Svg file will be generated relative to this
path.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Options
Svg conversion options.
An object or hashtable with follwing properties or keys:

| Property       | Description                                  |
| :------------: | :------------------------------------------- |
| \`background\`   | Diagram background color (default: white)    |
| \`fill_color\`   | Fill color for solid shapes (default: black) |
| \`font_family\`  | Text font (default: monospace)               |
| \`font_size\`    | Text font size (default 14)                  |
| \`scale\`        | Diagram scale (default: 1)                   |
| \`stroke_width\` | Stroke width for all lines (default: 2)      |

When using conversion projects instantiated by \`New-StaticHTMLSiteProject\` these
parameters are configured in \`Build.json\` parameter section \`svgbob\`.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### HTML fragment objects emitted by `Convert-MarkdownToHTMLFragment` with
### the `-Split` switch or equivalent objects.
## OUTPUTS

### Lines of Markdown text where all fenced code blocks labelled `bob` are
### replaced by Markdown style image links to svg files.
## NOTES
The svg conversion is performed by the external utility
\`svgbob.exe\` which is packaged with this module.
\`svgbob.exe\` is a \[Rust\](https://www.rust-lang.org/)
\[crate\](https://doc.rust-lang.org/rust-by-example/crates.html) which can be
installed from \[lib.rs\](https://lib.rs/crates/svgbob_cli).

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/Convert-SvgbobToSvg.html](https://wethat.github.io/MarkdownToHtml/2.5.0/Convert-SvgbobToSvg.html)

[[Svgbob](https://ivanceras.github.io/content/Svgbob.html)]()

