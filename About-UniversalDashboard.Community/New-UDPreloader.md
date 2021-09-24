---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDPreloader.md
schema: 2.0.0
---

# New-UDPreloader

## SYNOPSIS
Creates a new preloader.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDPreloader [-BackgroundColor <DashboardColor>] [-ProgressColor <DashboardColor>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDPreloader [-BackgroundColor <DashboardColor>] [-PercentComplete <Object>]
 [-ProgressColor <DashboardColor>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
New-UDPreloader [-Circular] [-Color <String>] [-Size <String>] [<CommonParameters>]
```

## DESCRIPTION
Creates a new preloader.
Preloaders can be used to show progress or indicate to the user something is processing.

## EXAMPLES

### Percent Complete
```
New-UDPreloader -PercentComplete 10
```

Creates a new determinate preloader with a percentage complete of 10.

### Indeterminate
```
New-UDPreloader -ProgressColor red
```

Creates a preloader with a progress color set to red.

### Circular
```
New-UDPreloader -Color blue -Circular
```

Creates a blue, circular preloader.

## PARAMETERS

### -BackgroundColor
The background color of the preloader

```yaml
Type: DashboardColor
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Circular
Whether the preloadre is circular.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color
The color of the preloader.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:
Accepted values: blue, red, green

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PercentComplete
The percent complete of the preloader.

```yaml
Type: Object
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProgressColor
The color of the preloaders progress.

```yaml
Type: DashboardColor
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Size
The size of the circular preloader.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:
Accepted values: small, medium, large

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
*

## RELATED LINKS
