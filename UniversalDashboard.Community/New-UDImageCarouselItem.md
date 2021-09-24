---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# New-UDImageCarouselItem

## SYNOPSIS
Create slide object for the image carousel component

## SYNTAX

```
New-UDImageCarouselItem [-Style <Hashtable>] [[-Id] <String>] [-ImageSource <String>] [[-Url] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Create slide for image carousel component, it support image url that host on the web or in local folders, it have alot of customization options.

## EXAMPLES

### Example 1
```
PS C:\> $Slide3 = @{
            BackgroundImage = 'https://stmed.net/sites/default/files/ultimate-spider-man-wallpapers-27724-2035627.jpg'
            BackgroundRepeat = 'no-repeat'
            BackgroundSize = 'cover'
            BackgroundPosition = '0% 0%'
            BackgroundColor  = '#3f51b5'
            Url  = 'http://Google.co.il'
        }
        New-UDCarousel -items {
            New-UDImageCarouselItem  @Slide3
        }
```



## PARAMETERS

### -Id
Set id for the carousel component, if not specified the value will be auto generated.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Url
Set the url that will be invoke when the button is click

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 11
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ImageSource


```yaml
Type: System.String
Parameter Sets: (All)
Aliases: BackgroundImage

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Style


```yaml
Type: System.Collections.Hashtable
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

### None
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
