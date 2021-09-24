---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# Show-UDToast

## SYNOPSIS
Shows a new toast message.

## SYNTAX

```
Show-UDToast [-BackgroundColor <DashboardColor>] [-Balloon] [-Broadcast] [-CloseOnClick] [-CloseOnEscape]
 [-Duration <Int32>] [-HideCloseButton] [<CommonParameters>]
```

## DESCRIPTION
Shows a new toast message.

## EXAMPLES

### Basic toast
```
New-UDButton -Text "Show Toast" -OnClick {
    Show-UDToast -Message 'Toast'
}
```

Shows a basic toast.

## PARAMETERS

### -BackgroundColor
Background color for the toast message.

```yaml
Type: DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Balloon
Whether the toast is a balloon format.

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

### -Broadcast
Sends a toast to all connected clients.

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

### -CloseOnClick
Whether the close the toast on click.

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

### -CloseOnEscape
Whether to close the toast on escape.

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

### -Duration
The number of milliseconds to show the toast message.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HideCloseButton
Whether to hide the close button.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### System.Object
## NOTES
*

## RELATED LINKS
