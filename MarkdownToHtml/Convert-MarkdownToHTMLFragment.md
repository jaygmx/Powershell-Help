---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/Convert-MarkdownToHTMLFragment.html
schema: 2.0.0
---

# Convert-MarkdownToHTMLFragment

## SYNOPSIS
Convert Markdown text to HTML fragments.

## SYNTAX

```
Convert-MarkdownToHTMLFragment [-InputObject] <Object> [[-IncludeExtension] <String[]>]
 [[-ExcludeExtension] <String[]>] [-Split] [<CommonParameters>]
```

## DESCRIPTION
Converts Markdown text to HTML fragments using configured
\[Markdown extensions\](about_MarkdownToHTML.md#supported-markdown-extensions).

## EXAMPLES

### EXAMPLE 1
```
Convert-MarkdownToHTMLFragment -Markdown '# Hello World'
```

Returns the HTML fragment object:

    Name               Value
    ----               -----
    HtmlFragment       \<h1 id="hello-world"\>Hello World\</h1\>...
    Title              Hello World

### EXAMPLE 2
```
Convert-MarkdownToHTMLFragment -Markdown '# Hello World' -Split
```

Returns the HTML fragment object:

    Name               Value
    ----               -----
    HtmlFragment       {\<h1 id="hello-world"\>,Hello World,\</h1\>,...}
    Title              Hello World

### EXAMPLE 3
```
Get-Item -LiteralPath "Convert-MarkdownToHTML.md" | Convert-MarkdownToHTMLFragment
```

Reads the content of Markdown file \`Example.md\` and returns a Html fragment object.

    Name               Value
    ----               -----
    Title              Convert-MarkdownToHTML
    HtmlFragment       \<h1 id="convert-Markdowntohtml"\>Convert-MarkdownToHTML\</h1\>...
    RelativePath       Convert-MarkdownToHTML.md

## PARAMETERS

### -InputObject
The input object can have one of the following types:
* An annotated \`\[System.IO.FileInfo\]\` object as emitted by \`Find-MarkdownFiles\`.
* A plain markdown string \[\`string\`\].
* A markdown descriptor object which is a \[\`hashtable\`\] with following contents:

  | Key            | Value Type | Description                                                   |
  | :------------- | :--------- | :------------------------------------------------------------ |
  | \`Markdown\`     | \[\`string\`\] | The markdown text. 
|
  | \`RelativePath\` | \[\`string\`\] | Relative path of the Markdown file below the input directory.
|

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases: Markdown

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IncludeExtension
Comma separated list of Markdown parsing extension names.
See \[Markdown extensions\](about_MarkdownToHTML.md#supported-markdown-extensions)
for an annotated list of supported extensions.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: @('advanced')
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExcludeExtension
Comma separated list of Markdown parsing extensions to exclude.
Mostly used when the the 'advanced' parsing option is included and
certain individual options need to be removed.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -Split
Split the Html fragment into an Array where each tag is in a separate slot.
This somewhat simplifies Html fragment post-processing.

For example the fragment

~~~ html
\<pre\>\<code class="language-PowerShell"\>PS&gt; Install-Module -Name MarkdownToHTML\</pre\>\</code\>
~~~

is split up into the array

| Index | Value                                        |
| :---: | :------------------------------------------- |
| 0     | \`\<pre\>\`                                      |
| 1     | \`\<code class="language-PowerShell"\>\`         |
| 2     | \`PS&gt; Install-Module -Name MarkdownToHTML\` |
| 3     | \`\</pre\>\`                                     |
| 4     | \`\</code\>\`                                    |

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

### Markdown text `[string]`, Markdown file `[System.IO.FileInfo]`,
### or a markdown descriptor `[hashtable]`.
## OUTPUTS

### HTML fragment object with following properties:
### | Property       | Description                                                         |
### | :------------: | :------------------------------------------------------------------ |
### | `Title`        | Optional page title. The first heading in the Markdown content.     |
### | `HtmlFragment` | The HTML fragment string or array generated from the Markdown text. |
### | `RelativePath` | Passed through from the input object, provided it exists.           |
## NOTES
The conversion to HTML fragments also includes:

* Changing links to Markdown files to the corresponding Html files.

  ~~~ Markdown
  \[Hello World\](Hello.md)
  ~~~

  becomes:

  ~~~ html
  \<a href="Hello.html"\>
  ~~~

* HTML encoding code blocks:

  ~~~ Markdown

  \`\`\`xml
  \<root\>
      \<thing/\>
  \</root\>

  \`\`\`
  ~~~

  becomes

  ~~~ HTML
  \<pre\>\<code class="language-xml"\>&lt;root&gt;
      &lt;thing/&gt;
  &lt;/root&gt;

  \</code\>\</pre\>
  ~~~

  which renders as

  \`\`\`xml
  \<root\>
      \<thing/\>
  \</root\>

  \`\`\`

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/Convert-MarkdownToHTMLFragment.html](https://wethat.github.io/MarkdownToHtml/2.5.0/Convert-MarkdownToHTMLFragment.html)

[`Convert-MarkdownToHTML`]()

[`Convert-SvgbobToSvg`]()

[`Find-MarkdownFiles`]()

[`Publish-StaticHtmlSite`]()

[`New-HTMLTemplate`]()

[[Markdown extensions](about_MarkdownToHTML.md#supported-markdown-extensions)]()

