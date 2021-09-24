---
external help file: MarkdownToHtml-help.xml
Module Name: MarkdownToHtml
online version: https://wethat.github.io/MarkdownToHtml/2.5.0/Find-MarkdownFiles.html
schema: 2.0.0
---

# Find-MarkdownFiles

## SYNOPSIS
Find all Markdown file below a given directory.

## SYNTAX

```
Find-MarkdownFiles [-Path] <String> [[-Exclude] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Recursively scans a directory and generates annotated \`\[System.IO.FileInfo\]\`
objects for each Markdown file.

The annotation is a \`NoteProperty\` named \`RelativePath\`.
It contains the
relative path of the Markdown file below the given directory.

## EXAMPLES

### EXAMPLE 1
```
Find-MarkdownFiles -Path '...\Modules\MarkdownToHtml' | Select-Object -Property Mode,LastWriteTime,Length,Name,RelativePath | Format-Table
```

Returns following annotated Markdown file objects of type \`\[System.IO.FileInfo\]\` for this PowerShell module:

    LastWriteTime        Length Name                       RelativePath
    -------------        ------ ----                       ------------
    13.09.2019 13:56:21  10751  Convert-MarkdownToHTML.md  Documentation\Convert-MarkdownToHTML.md
    13.09.2019 13:56:20   3348  MarkdownToHTML.md          Documentation\MarkdownToHTML.md
    13.09.2019 13:56:21   7193  New-HTMLTemplate.md        Documentation\New-HTMLTemplate.md
    11.09.2019 17:01:13   4455  README.md                  ReferenceData\katex\README.md
    ... 
... 
... 
...

## PARAMETERS

### -Path
Path to a directory containing Markdown files.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: True
```

### -Exclude
Omit the specified files.
Enter comma separated list of path elements or
patterns, such as "D*.md".
Wildcards are permitted.

```yaml
Type: System.String[]
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

### None
## OUTPUTS

### An `[System.IO.FileInfo]` object for each Markdown file found below
### the given directory. The emitted
### `[System.IO.FileInfo]` objects are annotated with a `NoteProperty` named
### `RelativePath` which specifies the relative path of the Markdown file below the
### directory specified in the `Path` parameter. The `RelativePath` property is
### **mandatory** if `Publish-StaticHtmlSite` is used in the downstream conversion
### pipeline to generate HTML files in the correct locations.
## NOTES

## RELATED LINKS

[https://wethat.github.io/MarkdownToHtml/2.5.0/Find-MarkdownFiles.html](https://wethat.github.io/MarkdownToHtml/2.5.0/Find-MarkdownFiles.html)

[`Convert-MarkdownToHTML`]()

[`Convert-MarkdownToHTMLFragment`]()

[`Publish-StaticHtmlSite`]()

[`New-HTMLTemplate`]()

