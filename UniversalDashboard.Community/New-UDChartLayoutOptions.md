---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDCard.md
schema: 2.0.0
---

# New-UDChartLayoutOptions

## SYNOPSIS
Layout options for a chart.

## SYNTAX

### Size
```
New-UDChartLayoutOptions -Padding <Int32> [<CommonParameters>]
```

### Object
```
New-UDChartLayoutOptions -PaddingLeft <Int32> -PaddingRight <Int32> -PaddingTop <Int32> -PaddingBottom <Int32>
 [<CommonParameters>]
```

## DESCRIPTION
Layout options for a chart.

## EXAMPLES

### Example 1
```
PS C:\> $LayoutOptions = New-UDLayoutOptions -Padding 15
PS C:\> $Options = New-UDChartOptions -LayoutOptions $LayoutOptions
```

Creates chart options with layout options set to a padding for 15.

## PARAMETERS

### -Padding
The padding to add inside the chart.

```yaml
Type: System.Int32
Parameter Sets: Size
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PaddingBottom
The padding to add inside the bottom of the chart.

```yaml
Type: System.Int32
Parameter Sets: Object
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PaddingLeft
The padding to add inside the left of the chart.

```yaml
Type: System.Int32
Parameter Sets: Object
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PaddingRight
The padding to add inside the right of the chart.

```yaml
Type: System.Int32
Parameter Sets: Object
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PaddingTop
The padding to add inside the top of the chart.

```yaml
Type: System.Int32
Parameter Sets: Object
Aliases:

Required: True
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
