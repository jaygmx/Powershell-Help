---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDCard.md
schema: 2.0.0
---

# New-UDChartTitleOptions

## SYNOPSIS
Title options for a chart.

## SYNTAX

```
New-UDChartTitleOptions [-Display] [[-Position] <String>] [[-FontSize] <Int32>] [[-FontStyle] <String>]
 [[-FontFamily] <String>] [[-Padding] <Int32>] [[-FontColor] <DashboardColor>] [[-LineHeight] <Single>]
 [[-Text] <String>] [<CommonParameters>]
```

## DESCRIPTION
Title options for a chart.

## EXAMPLES

### Example 1
```
PS C:\> $TitleOptions =  New-UDChartTitleOptions -Display -Text "Fruit Chart"
PS C:\> $Options = New-UDChartOptions -TitleOptions $TitleOptions
PS C:\> New-UDChart -Options $Options #...
```

Creates a new chart and specifies a title for the chart.

## PARAMETERS

### -Display
Displays the title.

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

### -FontColor
Font color

```yaml
Type: UniversalDashboard.Models.DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontFamily
Font family

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

### -FontSize
Font size

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontStyle
Font style

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, bold, italic

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LineHeight
Height of an individual line of text

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

### -Padding
Number of pixels to add above and below the title text.

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

### -Position
Position of title.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: top, bottom, left, right

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text
Title text to display.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
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
