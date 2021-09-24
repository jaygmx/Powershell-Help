---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDImage

## SYNOPSIS
This commandlet output image in markdown syntax

## SYNTAX

### Source
```
New-MDImage [[-Source] <String>] [-Title <String>] [-AltText <String>] [-Link <String>] [<CommonParameters>]
```

### Shields.io
```
New-MDImage [-Title <String>] [-AltText <String>] [-Subject <String>] [-Status <String>] [-Color <String>]
 [-Style <String>] [-Link <String>] [<CommonParameters>]
```

## DESCRIPTION
This commandlet output image in markdown syntax like this !\[alt text\](link "title")

## EXAMPLES

### EXAMPLE 1
```
New-MDImage -Link "example.png"
"example.png" | New-MDImage
```

!\[\](example.png)

### EXAMPLE 2
```
New-MDImage -Link "example.png" -Title "Example"
"example.png" | New-MDImage -Title "Example"
```

!\[\](example.png "Example")

### EXAMPLE 3
```
New-MDImage -Link "example.png" -Title "Example" -AltText "Failed to load"
"example.png" | New-MDImage -Title "Example" -AltText "Failed to load"
```

!\[Failed to load\](example.png "Example")

### EXAMPLE 4
```
New-MDImage -Subject "SUBJECT" -Status "STATUS" -Color "green"
```

!\[\](https://img.shields.io/badge/SUBJECT-STATUS-green.svg)

## PARAMETERS

### -Source
Text that represents the image source

```yaml
Type: System.String
Parameter Sets: Source
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Title
The title of the image

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

### -AltText
The alternative text of the image

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

### -Subject
The \<SUBJECT\> in https://img.shields.io/badge/\<SUBJECT\>-\<STATUS\>-\<COLOR\>.svg

```yaml
Type: System.String
Parameter Sets: Shields.io
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
{{ Fill Status Description }}

```yaml
Type: System.String
Parameter Sets: Shields.io
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color
The \<Color\> in https://img.shields.io/badge/\<SUBJECT\>-\<STATUS\>-\<COLOR\>.svg
One of the brightgreen, green, yellowgreen, yellow, orange, red, lightgrey, blue

```yaml
Type: System.String
Parameter Sets: Shields.io
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Style
The \<STYLE\> in https://img.shields.io/badge/\<SUBJECT\>-\<STATUS\>-\<COLOR\>.svg

```yaml
Type: System.String
Parameter Sets: Shields.io
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Link
Add a link to the image

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

### Any text representing link or parameters to drive shields.io badges
## OUTPUTS

### The image construct in markdown
## NOTES

## RELATED LINKS

[New-MDLink
https://help.github.com/articles/basic-writing-and-formatting-syntax/
https://img.shields.io/badge/<SUBJECT>-<STATUS>-<COLOR>.svg
http://shields.io/]()

