---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDCollapsible.md
schema: 2.0.0
---

# New-UDCollapsibleItem

## SYNOPSIS
Creates a collapsible item.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDCollapsibleItem [-Active] [-AutoRefresh] [-BackgroundColor <DashboardColor>] [-Endpoint <Object>]
 [-FontColor <DashboardColor>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDCollapsibleItem [-Active] [-BackgroundColor <DashboardColor>] [-Content <ScriptBlock>]
 [-FontColor <DashboardColor>] [<CommonParameters>]
```

## DESCRIPTION
Creates a collapsible item.
Use with New-UDCollapsible.
This will create a single item within the collapsible.

## EXAMPLES

### Example 1
```
PS C:\> New-UDCollapsible -Id "Collapsible" -Items {
                New-UDCollapsibleItem -Title "First" -Icon user -Content {
                    New-UDCard -Title "First"
                } -Active
                New-UDCollapsibleItem -Title "Second" -Icon group -Content {
                    New-UDCard -Title "Second"
                }
                New-UDCollapsibleItem -Title "Third" -Icon user -Content {
                    New-UDCard -Title "Third"
                }
            }
```

Creates a new collapsible with 3 different items.

## PARAMETERS

### -Active
Specifies whether the item is active by default.
This will expand the item.

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

### -AutoRefresh
Specifies that this component auto-refreshs on the RefreshInterval.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
Background color of the component item.

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

### -Content
Content of this collapsible.
Other components can be nested within this item.

```yaml
Type: ScriptBlock
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Endpoint
The endpoint that returns the content for this component.

```yaml
Type: Object
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontColor
Font color of the component item.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
