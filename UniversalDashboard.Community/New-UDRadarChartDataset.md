---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDPreloader.md
schema: 2.0.0
---

# New-UDRadarChartDataset

## SYNOPSIS
Creates a dataset for a radar chart.

## SYNTAX

```
New-UDRadarChartDataset [[-DataProperty] <String>] [[-Label] <String>] [[-BackgroundColor] <DashboardColor[]>]
 [[-BorderColor] <DashboardColor[]>] [[-BorderWidth] <Int32>] [[-BorderCapStyle] <String>]
 [[-BorderJoinStyle] <String>] [[-Fill] <Object>] [[-LineTension] <Int32>]
 [[-PointBackgroundColor] <DashboardColor[]>] [[-PointBorderColor] <DashboardColor[]>]
 [[-PointBorderWidth] <Int32[]>] [[-PointRadius] <Int32[]>] [[-PointStyle] <String[]>]
 [[-PointHitRadius] <Int32[]>] [[-PointHoverBackgroundColor] <DashboardColor[]>]
 [[-PointHoverBorderColor] <DashboardColor[]>] [[-PointHoverBorderWidth] <Int32[]>]
 [[-PointHoverRadius] <Int32[]>] [<CommonParameters>]
```

## DESCRIPTION
Creates a dataset for a radar chart.

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -BackgroundColor
The fill color under the line

```yaml
Type: UniversalDashboard.Models.DashboardColor[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderCapStyle
Cap style of the line.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: butt, round, square

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderColor
The color of the line.

```yaml
Type: UniversalDashboard.Models.DashboardColor[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderJoinStyle
Line joint style.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: bevel, round, miter

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderWidth
The width of the line in pixels.

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

### -DataProperty
The property of the object to use as the y-Axis of the dataset.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Fill
How to fill the area under the line.

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

### -Label
The label for the dataset which appears in the legend and tooltips.

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

### -LineTension
Bezier curve tension of the line.
Set to 0 to draw straightlines.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointBackgroundColor
The fill color for points.

```yaml
Type: UniversalDashboard.Models.DashboardColor[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointBorderColor
The border color for points.

```yaml
Type: UniversalDashboard.Models.DashboardColor[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointBorderWidth
The width of the point border in pixels.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 11
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointHitRadius
The pixel size of the non-displayed point that reacts to mouse events.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 14
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointHoverBackgroundColor
Point background color when hovered.

```yaml
Type: UniversalDashboard.Models.DashboardColor[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 15
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointHoverBorderColor
Point border color when hovered.

```yaml
Type: UniversalDashboard.Models.DashboardColor[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 16
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointHoverBorderWidth
Border width of point when hovered.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 17
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointHoverRadius
The radius of the point when hovered.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 18
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointRadius
The radius of the point shape.
If set to 0, the point is not rendered.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 12
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PointStyle
Style of the point.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:
Accepted values: circle, cross, crossRot, dash, line, rect, rectRounded, rectRot, star, triangle

Required: False
Position: 13
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
