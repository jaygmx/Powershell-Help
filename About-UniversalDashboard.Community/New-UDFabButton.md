---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDFab.md
schema: 2.0.0
---

# New-UDFabButton

## SYNOPSIS
Creates a floating action button within a FAB.

## SYNTAX

```
New-UDFabButton [[-ButtonColor] <DashboardColor>] [<CommonParameters>]
```

## DESCRIPTION
Creates a floating action button within a FAB.

## EXAMPLES

### Example 1
```
PS C:\> New-UdFab -Id "main" -Icon "plus" -Size "large" -ButtonColor "red" -Content {
                New-UDFabButton -ButtonColor "green" -Icon "edit" -size "small"
                New-UDFabButton -Id "btn" -ButtonColor "yellow" -Icon "trash" -size "large" -onClick {
                    Show-UDToast -Message "Clicked!"
                }
            }
```

Creates two FAB buttons within a FAB with custom icons and colors and an event handler.

## PARAMETERS

### -ButtonColor
The color of the button.

```yaml
Type: DashboardColor
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

## OUTPUTS

## NOTES

## RELATED LINKS
