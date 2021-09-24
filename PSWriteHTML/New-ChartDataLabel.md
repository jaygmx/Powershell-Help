---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-ChartDataLabel

## SYNOPSIS
Configures DataLabels for Charts

## SYNTAX

```
New-ChartDataLabel [-Enabled] [[-TextAnchor] <String>] [-Distributed] [[-OffsetX] <Int32>] [[-OffsetY] <Int32>]
 [[-FontSize] <Object>] [[-FontFamily] <String>] [[-FontColor] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Configures DataLabels for Charts

## EXAMPLES

### EXAMPLE 1
```
An example
```

## PARAMETERS

### -Enabled
To determine whether to show dataLabels or not

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

### -TextAnchor
The alignment of text relative to dataLabel's drawing position.
Accepted values: start, middle, end

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

### -Distributed
Similar to plotOptions.bar.distributed, this option makes each data-label discrete.
So, when you provide an array of colors in datalabels.style.colors, the index in the colors array correlates with individual data-label index of all series.

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

### -OffsetX
Sets the left offset for dataLabels

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases: DataLabelsOffsetX

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OffsetY
Sets the top offset for dataLabels

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontSize
FontSize for the label

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases: DataLabelsFontSize

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontFamily
FontFamily for the label

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontColor
FontColors for the dataLabels.
Accepts an array of string colors.
Each index in the array corresponds to the series

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: DataLabelsColor

Required: False
Position: 6
Default value: None
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
