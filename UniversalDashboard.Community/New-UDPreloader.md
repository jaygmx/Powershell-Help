---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDPreloader.md
schema: 2.0.0
---

# New-UDPreloader

## SYNOPSIS
Creates a new preloader.

## SYNTAX

### indeterminate (Default)
```
New-UDPreloader [-BackgroundColor <DashboardColor>] [-ProgressColor <DashboardColor>] [<CommonParameters>]
```

### determinate
```
New-UDPreloader [-PercentComplete <Object>] [-BackgroundColor <DashboardColor>]
 [-ProgressColor <DashboardColor>] [<CommonParameters>]
```

### circular
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
Type: UniversalDashboard.Models.DashboardColor
Parameter Sets: indeterminate, determinate
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: circular
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
Type: System.String
Parameter Sets: circular
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
Type: System.Object
Parameter Sets: determinate
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
Type: UniversalDashboard.Models.DashboardColor
Parameter Sets: indeterminate, determinate
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
Type: System.String
Parameter Sets: circular
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

## RELATED LINKS
