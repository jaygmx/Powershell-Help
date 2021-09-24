---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDLink.md
schema: 2.0.0
---

# New-UDPolarChartOptions

## SYNOPSIS
Chart options for a polar area chart.

## SYNTAX

```
New-UDPolarChartOptions [[-LayoutOptions] <Object>] [[-LegendOptions] <Object>] [[-TitleOptions] <Object>]
 [[-TooltipOptions] <Object>] [[-xAxes] <Object>] [[-yAxes] <Object>] [[-StartAngle] <Single>]
 [[-AnimateRotate] <Boolean>] [[-AnimateScale] <Boolean>] [<CommonParameters>]
```

## DESCRIPTION
Chart options for a polar area chart.

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -AnimateRotate
If true, the chart will animate in with a rotation animation.

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AnimateScale
If true, will animate scaling the chart from the center outwards.

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LayoutOptions
Layout options for this chart.
Use New-UDChartLayoutOptions.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LegendOptions
Legend options for this chart.
Use New-UDChartLegendOptions.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartAngle
Starting angle to draw arcs for the first item in a dataset.

```yaml
Type: System.Single
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleOptions
Title options for this chart.
Use New-UDChartTitleOptions.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TooltipOptions
Tooltip options for this chart.
Use New-UDChartTooltipOptions.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -xAxes
The x-Axis for this chart.
Use New-UDCategoryChartAxis, New-UDLinearChartAxis or New-UDLogarithmicChartAxis.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -yAxes
The y-Axis for this chart.
Use New-UDCategoryChartAxis, New-UDLinearChartAxis or New-UDLogarithmicChartAxis.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
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
