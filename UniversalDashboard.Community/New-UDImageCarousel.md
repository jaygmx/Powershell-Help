---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDImageCarousel.md
schema: 2.0.0
---

# New-UDImageCarousel

## SYNOPSIS
Render image carousel in dashboard

## SYNTAX

```
New-UDImageCarousel [[-Items] <ScriptBlock>] [[-Id] <String>] [-Indicators] [-FullScreen] [-Interval <Int32>]
 [-Duration <Int32>] [[-Height] <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Add image carousel to UniversalDashboard you can set the carousel to be full screen width and add button that update it href automatic to the url that set for every slide and more..

## EXAMPLES

### Example 1
```
New-UDImageCarousel -Items {
        New-UDImageCarouselItem -ImageSource https://hdqwalls.com/wallpapers/deadpool-baby-yoda-c6.jpg -Url 'https://hdqwalls.com/wallpapers/deadpool-baby-yoda-c6.jpg'
        New-UDImageCarouselItem -ImageSource https://hdqwalls.com/wallpapers/black-widow4k-5b.jpg -Url 'https://hdqwalls.com/wallpapers/black-widow4k-5b.jpg'
        New-UDImageCarouselItem -ImageSource https://hdqwalls.com/wallpapers/batman-fire-4k-xv.jpg -Url 'https://hdqwalls.com/wallpapers/batman-fire-4k-xv.jpg'
} -Indicators
```

Create new image carousel with 3 slides and with fixed button on every slide.

## PARAMETERS

### -Height
Set the main carousel container height

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Set id for the carousel component, if not specified the value will be auto generated.

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

### -Items
The items (slides) to add to the carousel container, the items need to be created using New-UDImageCarouselItem cmdlet

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Duration
{{ Fill Duration Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FullScreen
{{ Fill FullScreen Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: FullWidth

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Indicators
{{ Fill Indicators Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: ShowIndicators

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Interval
{{ Fill Interval Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases: Speed

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
