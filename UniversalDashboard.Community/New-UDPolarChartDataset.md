---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDLink.md
schema: 2.0.0
---

# New-UDPolarChartDataset

## SYNOPSIS
Creates a dataset for a polar area chart.

## SYNTAX

```
New-UDPolarChartDataset [[-DataProperty] <String>] [[-Label] <String>] [[-BackgroundColor] <DashboardColor[]>]
 [[-BorderColor] <DashboardColor[]>] [[-BorderWidth] <Int32>] [[-HoverBackgroundColor] <DashboardColor[]>]
 [[-HoverBorderColor] <DashboardColor[]>] [[-HoverBorderWidth] <Int32[]>] [<CommonParameters>]
```

## DESCRIPTION
Polar area charts are similar to pie charts, but each segment has the same angle - the radius of the segment differs depending on the value.

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -BackgroundColor
The fill color of the arcs in the dataset.

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

### -BorderColor
The border color of the arcs in the dataset.

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

### -BorderWidth
The border width of the arcs in the dataset.

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

### -HoverBackgroundColor
The fill colour of the arcs when hovered.

```yaml
Type: UniversalDashboard.Models.DashboardColor[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HoverBorderColor
The stroke colour of the arcs when hovered.

```yaml
Type: UniversalDashboard.Models.DashboardColor[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HoverBorderWidth
The stroke width of the arcs when hovered.

```yaml
Type: System.Int32[]
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
