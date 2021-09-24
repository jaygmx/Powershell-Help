---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDButton.md
schema: 2.0.0
---

# New-UDButton

## SYNOPSIS
Creates a new button.

## SYNTAX

```
New-UDButton [[-BackgroundColor] <DashboardColor>] [[-FontColor] <DashboardColor>] [-Disabled] [-Flat]
 [-Floating] [<CommonParameters>]
```

## DESCRIPTION
Creates a new button.
Buttons come in different shapes and sizes and can be configured to execute scripts when clicked.

## EXAMPLES

### Raised Button
```
New-UDButton -Text "Button"
```

Creates a basic, raised button.

### Button with Icon
```
New-UDButton -Text "Button" -Icon cloud
```

Creates a basic, raised button with an icon.

### Button Colors
```
New-UDButton -Text "Button" -BackgroundColor "red" -FontColor "white"
```

Creates a red button with white text.

### Floating
```
New-UDButton -Floating -Icon plus
```

Creates a circular, floating button with a plus icon.

### Flat
```
New-UDButton -Flat -Text "Button"
```

Creates a flat button

### OnClick Event Handler
```
New-UDButton -Text "Button" -OnClick {
    Show-UDToast -Message "Ouch!"
}
```

Creats a button that shows a toast message when clicked.

### Button sizes
```
`
New-UDButton -Text "Big" -Height 300 -Width "100%"
```

\`

Creates a button with height of 300px and 100% width. 
Note: the "px" will be appended automatically if not specified.

### Custom styles
```
`
New-UDButton -Text "Custom" -Style @{
    Font-Size = 36 px
    Height = 300 px
}
```

\`

Creates a button, with font-size 36 and height of 300 pixels.
Will be prioritized over the -height param.

## PARAMETERS

### -BackgroundColor
Background color of the button.

```yaml
Type: DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Disabled
Creates a disabled button.

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

### -Flat
Creates a flat button without shadows.

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

### -Floating
Creates a circular, floating button.

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

### -FontColor
Font color of the button.
This also changes the icon color.

```yaml
Type: DashboardColor
Parameter Sets: (All)
Aliases:

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

## RELATED LINKS
