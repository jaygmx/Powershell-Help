---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDSelect.md
schema: 2.0.0
---

# New-UDSplitPane

## SYNOPSIS
Creates a split pane between two controls that you can adjust the size of.

## SYNTAX

```
New-UDSplitPane [[-Id] <String>] [-Content] <ScriptBlock> [[-Direction] <String>] [[-MinimumSize] <Int32>]
 [[-DefaultSize] <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Creates a split pane between two controls that you can adjust the size of.

## EXAMPLES

### Vertical Pane
```
New-UDSplitPane -Content {
    New-UDCard -Title 'Side 1' -Content {}
    New-UDCard -Title 'Side 2' -Content {}
}
```

Creates a vertical split pane.

### Horizontal Pane
```
New-UDSplitPane -Content {
    New-UDCard -Title 'Side 1' -Content {}
    New-UDCard -Title 'Side 2' -Content {}
} -Direction horizontal
```

Creates a horizontal split pane.

## PARAMETERS

### -Content
The controls to create the split pane for.
This is should contain exactly two controls.

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultSize
The default size in pixels of the top or left component.

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

### -Direction
Whether you want a split panel that is vertical or horizontal

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: vertical, horizontal

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Id of the split pane.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MinimumSize
Minimum size in pixels of the panes.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
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
