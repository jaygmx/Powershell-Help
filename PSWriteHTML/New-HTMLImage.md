---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLImage

## SYNOPSIS
Creates IMG tag with image link or image bundled inline

## SYNTAX

```
New-HTMLImage [[-Source] <String>] [[-UrlLink] <Uri>] [[-AlternativeText] <String>] [[-Class] <String>]
 [[-Target] <String>] [[-Width] <Object>] [[-Height] <Object>] [-Inline] [-DisableCache] [<CommonParameters>]
```

## DESCRIPTION
Creates IMG tag with image link or image bundled inline

## EXAMPLES

### EXAMPLE 1
```
New-HTMLImage -Source 'https://evotec.pl/image.png' -UrlLink 'https://evotec.pl/' -AlternativeText 'My other text' -Class 'otehr' -Width '100%'
```

## PARAMETERS

### -Source
Link to an image or file path to an image

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UrlLink
Specifies the URL of the page the link goes to when user clicks an image

```yaml
Type: System.Uri
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlternativeText
Specifies an alternate text for the image, if the image for some reason cannot be displayed

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Class
Overwrites default CSS settings for links

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: Logo
Accept pipeline input: False
Accept wildcard characters: False
```

### -Target
The target attribute specifies where to open the linked document.

- _blank	Opens the linked document in a new window or tab
- _self	Opens the linked document in the same frame as it was clicked (this is default)
- _parent	Opens the linked document in the parent frame
- _top	Opens the linked document in the full body of the window

Additionally framename can be given.
Default is _blank

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: _blank
Accept pipeline input: False
Accept wildcard characters: False
```

### -Width
Width of an image (optional)

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Height
Height of an image (optional)

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Inline
Inserts given Image URL/File directly into HTML

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

### -DisableCache


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

## OUTPUTS

## NOTES
General notes

## RELATED LINKS
