---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/New-HTMLTemplate.html
schema: 2.0.0
---

# New-HTMLTemplate

## SYNOPSIS
Create a customizable template directory for building HTML files from
Markdown files.

## SYNTAX

```
New-HTMLTemplate [-Destination] <String> [<CommonParameters>]
```

## DESCRIPTION
The factory-default conversion template is copied to the destination directory
to seed the customization process.
The new template directory contains the
resources necesssary to generate fully functional, standalone HTML files.

See
\[Conversion Template Customization\](about_MarkdownToHTML.md#conversion-template-customization)
for ways to customize the template.

## EXAMPLES

### EXAMPLE 1
```
New-HTMLTemplate -Destination 'E:\MyTemplate'
```

Create a copy of the factory template in \`E:\MyTemplate\` for customization.

## PARAMETERS

### -Destination
Location of the new conversion template directory.
The template directory
should be empty or non-existent.

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

### This function does not read from the pipe.
## OUTPUTS

### The new conversion template directory `[System.IO.DirectoryInfo]`.
## NOTES

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/New-HTMLTemplate.html](https://wethat.github.io/MarkdownToHtml/2.5.0/New-HTMLTemplate.html)

[`New-StaticHTMLSiteProject`]()

