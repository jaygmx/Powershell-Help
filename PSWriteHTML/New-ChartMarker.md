---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-ChartMarker

## SYNOPSIS
Short description

## SYNTAX

```
New-ChartMarker [[-Size] <Int32>] [[-Color] <String[]>] [[-StrokeColors] <String[]>] [[-StrokeWidth] <Int32[]>]
 [[-StrokeOpacity] <Int32[]>] [[-StrokeDashArray] <Int32[]>] [[-FillOpacity] <Int32[]>] [[-Shape] <String[]>]
 [[-Radius] <Int32[]>] [[-OffsetX] <Int32[]>] [[-OffsetY] <Int32[]>] [-ShowNullDataPoints]
 [[-HoverSize] <Int32[]>] [[-HoverSizeOffset] <Int32[]>] [<CommonParameters>]
```

## DESCRIPTION
Long description

## EXAMPLES

### EXAMPLE 1
```
New-HTMLChart -Title 'Incidents Reported vs Solved' -TitleAlignment center {
    New-ChartMarker -Size 30 -Color red -Shape square -StrokeColors yellow
}
```

## PARAMETERS

### -Size
Size of the marker point.

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color
Sets the fill color(s) of the marker point.

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

### -StrokeColors
Stroke Color of the marker.
Accepts a single color or an array of colors in a multi-series chart.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StrokeWidth
Stroke Size of the marker.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StrokeOpacity
Opacity of the border around marker.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StrokeDashArray
Dashes in the border around marker.
Higher number creates more space between dashes in the border.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FillOpacity
Opacity of the marker fill color.

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

### -Shape
Shape of the marker.
Available Options for shape circle or square

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Radius
Radius of the marker (applies to square shape)

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OffsetX
Sets the left offset of the marker

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OffsetY
Sets the top offset of the marker

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

### -ShowNullDataPoints
Whether to show markers for null values in a line/area chart.
If disabled, any null values present in line/area charts will not be visible.

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

### -HoverSize
Fixed size of the marker when it is active

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

### -HoverSizeOffset
Unlike the fixed size, this option takes the original markers.size and increases/decreases the value based on it.
So, if markers.size: 6, markers.hover.sizeOffset: 3 will make the marker's size 9 when hovered.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 13
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Based on https://apexcharts.com/docs/options/markers/

## RELATED LINKS
