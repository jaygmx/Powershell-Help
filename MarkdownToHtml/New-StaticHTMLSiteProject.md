---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/New-StaticHTMLSiteProject.html
schema: 2.0.0
---

# New-StaticHTMLSiteProject

## SYNOPSIS
Create a customizable Markdown to HTML site conversion project.

## SYNTAX

```
New-StaticHTMLSiteProject [-ProjectDirectory] <String> [<CommonParameters>]
```

## DESCRIPTION
Create a new static HTML site project directoy with some default content
ready for building.

A single markdown file (\`README.md\`) is provided as initial content.
It explains
some customization options and the typical site authoring process.
It is recommended to build the project by executing its build script
\`Build.ps1\`.
This creates the initial static HTML site with the HTML version of
the README (\`docs/README.html\`) which is more pleasant to read also showcases
some features.

See \[Project Customization\](about_MarkdownToHTML.md#static-site-project-customization)
for details about the project directory structure and site customization.

## EXAMPLES

### EXAMPLE 1
```
New-StaticHTMLSiteProject -ProjectDirectory MyProject
```

Create a new conversion project names 'MyProject' in the current directory.
The
project is ready for build.

## PARAMETERS

### -ProjectDirectory
The location of the new Markdown to HTML site conversion project.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### The new project directory object `[System.IO.DirectoryInfo]`
## NOTES

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/New-StaticHTMLSiteProject.html](https://wethat.github.io/MarkdownToHtml/2.5.0/New-StaticHTMLSiteProject.html)

[`New-HTMLTemplate`]()

[[Project Customization](about_MarkdownToHTML.md#static-site-project-customization)]()

