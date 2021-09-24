---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/New-PageHeadingNavigation.html
schema: 2.0.0
---

# New-PageHeadingNavigation

## SYNOPSIS
Generate navigation specifications for specified headings found in an HTML
fragment.

## SYNTAX

```
New-PageHeadingNavigation [-HTMLfragment] <String> [[-NavTemplate] <Object>] [[-HeadingLevels] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Generates a link specification for each heading in an HTML fragment which
* has an \`id\` attribute
* matches heading level constraint

The link specifications have the format required by \`ConvertTo-NavigationItem\`
to generate navigation bar items.

## EXAMPLES

### EXAMPLE 1
```
New-PageHeadingNavigation $fragment -HeadingLevels '234'
```

Create an HTML element for navigation to page headings \`\<h2\>\`, \`\<h3\>\`, \`\<h4\>\`.
All other headings are ignored.
\`$fragment\` is a HTML framgment defined as:

~~~ PowerShell
$fragment = '\<h2 id="bob"\>Hello World\</h2\>'
~~~

Output:

~~~ HTML
\<button class="navitem"\>
   \<a href="#bob"\>\<span class="navitem2"\>Hello World\</span\>\</a\>
\</button\>
~~~

Note that the heading level has been added to the css class.

### EXAMPLE 2
```
Hello World</h2>' -NavTemplate $custom
```

Create an HTML element for navigation to an heading using the custom template \`$custom\`.

~~~ PowerShell
    $custom = @{ navheading = '\<span class="li-item{{level}}"\>{{navtext}}\</span\>'}
~~~

Output:

~~~ HTML
\<button class="navitem"\>
    \<a href="#bob"\>\<span class="li-item2"\>Hello World\</span\>\</a\>
\</button\>
~~~

Note that the heading level is used as a postfix for the css class.

## PARAMETERS

### -HTMLfragment
HTML fragment to scan for headings.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NavTemplate
An optional dictionary of the named HTML template needed to add a heading
link to the navigation bar.

+ :--------: + :----------: + ----------------------------------------
| Type       | Key          | HTML Template
+ ========== + ============ + ========================================
| Heading    | "navheading" | ~~~ html
| link       |              |\<span class='navitem{{level}}'\>{{navtext}}\</span\>"
| template   |              | ~~~
+ ---------- + ------------ + ----------------------------------------

The HTML template above is the value defined in
\`Build.json\`.
That value is used if the given dictionary does not define the
"navheading" mapping or if no dictionary is given at all.
Additional mappings
contained in the dictionary are ignored.

For more customization options see
\[Static Site Project Customization\](about_MarkdownToHTML.md#static-site-project-customization).

The css styles used in the template is defined in \`md-styles.css\`.

Following placeholders in the HTML template are recognized.

| Placeholder   | Description
| :-----------: | -----------
| \`{{level}}\`   | heading level.
| \`{{navtext}}\` | heading text

During the build process the placeholders are replaced with content taken from
the \`NavSpec\` parameter.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: $SCRIPT:defaultNavTemplate
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeadingLevels
A string of numbers denoting the levels of the headings to add to the navigation
bar.
By default the headings at level 1,2 and 3 are added to the Navigation bar.
If headings should not be automatically added to the navigation bar, use the
empty string \`''\` for this parameter.
If omitted, the default configuration
defined by option "capture_page_headings" in \`Build.json\` is used.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 123
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None. This function does not read from a pipe.
## OUTPUTS

### HTML elements representing navigation links to headings on the input HTML
### fragment for use in the navigation bar of sites created by
### `New-StaticHTMLSiteProject`.
## NOTES
This function is typically used in the build script \`Build.ps1\` to define
the contents of the navigation bar (placeholder \`{{nav}}\`).

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/New-PageHeadingNavigation.html](https://wethat.github.io/MarkdownToHtml/2.5.0/New-PageHeadingNavigation.html)

[`New-StaticHTMLSiteProject`]()

[`ConvertTo-NavigationItem`]()

