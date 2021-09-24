---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDIcon.md
schema: 2.0.0
---

# New-UDIcon

## SYNOPSIS
Create icon from the FontAwesome pack

## SYNTAX

```
New-UDIcon [[-Color] <DashboardColor>] [[-ClassName] <String>] [[-Flip] <String>] [-Border] [-FixedWidth]
 [<CommonParameters>]
```

## DESCRIPTION
This command will generate an svg icon from the FontAwesome library, this icons comes from the Solid,Brand and regular packages.
The library include 1300+ icons.

## EXAMPLES

### Example 1
```
New-UDIcon -Icon box -Style @{color = '#000'} -Id 'test-icon-button'
```

Create icon with the default size sm and it has black color.

### Example 2
```
New-UDIcon -Icon spinner -Size 3x -Style @{color = '#000'} -Id 'test-icon-button' -Spin
```

Create icon that has spin animation.

### Example 3
```
New-UDIcon -Icon angry -Size 3x -Style @{color = '#000'} -Id 'test-icon-button' -Regular
```

Create angry icon that have a size of 3 and black color, and also this icon is from the FontAwesome regular pack ( semi light ) style.

## PARAMETERS

### -Border
set square border around the icon

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClassName
Add custom css class name

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color
The color of the icon.

```yaml
Type: DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FixedWidth
set the icons to the same fixed width

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Flip
Flip horizontally, vertically, or both

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Accepted values: horizontal, vertical, both

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
