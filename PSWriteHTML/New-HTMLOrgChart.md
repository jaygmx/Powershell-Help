---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLOrgChart

## SYNOPSIS
Short description

## SYNTAX

```
New-HTMLOrgChart [[-ChartNodes] <ScriptBlock>] [[-Direction] <String>] [[-VisileLevel] <Int32>]
 [[-VerticalLevel] <Int32>] [[-NodeTitle] <String>] [-ToggleSiblings] [-Pan] [-Zoom] [[-ZoomInLimit] <Double>]
 [[-ZoomOutLimit] <Double>] [-Draggable] [-AllowExport] [[-ExportFileName] <String>]
 [[-ExportExtension] <Object>] [[-ChartID] <String>] [<CommonParameters>]
```

## DESCRIPTION
Long description

## EXAMPLES

### EXAMPLE 1
```
New-HTML {
    New-HTMLOrgChart {
        New-OrgChartNode -Name 'Test' -Title 'Test2' {
            New-OrgChartNode -Name 'Test' -Title 'Test2'
            New-OrgChartNode -Name 'Test' -Title 'Test2'
            New-OrgChartNode -Name 'Test' -Title 'Test2' {
                New-OrgChartNode -Name 'Test' -Title 'Test2'
            }
        }
    } -AllowExport -ExportExtension pdf -Draggable
} -FilePath $PSScriptRoot\Example-OrgChart01.html -ShowHTML -Online
```

## PARAMETERS

### -ChartNodes
Define nodes to be shown on the chart

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Direction
The available values are "top to bottom" (default value), "bottom to top", "left to right" and "right to left"

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VisileLevel
It indicates the level that at the very beginning orgchart is expanded to.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -VerticalLevel
Users can make use of this option to align the nodes vertically from the specified level.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -NodeTitle
It sets one property of datasource as text content of title section of orgchart node.
In fact, users can create a simple orghcart with only nodeTitle option.

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

### -ToggleSiblings
Once enable this option, users can show/hide left/right sibling nodes respectively by clicking left/right arrow.

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

### -Pan
Users could pan the orgchart by mouse drag&drop if they enable this option.

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

### -Zoom
Users could zoomin/zoomout the orgchart by mouse wheel if they enable this option.

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

### -ZoomInLimit
Users are allowed to set a zoom-in limit.

```yaml
Type: System.Double
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ZoomOutLimit
Users are allowed to set a zoom-out limit.

```yaml
Type: System.Double
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Draggable
Users can drag & drop the nodes of orgchart if they enable this option.
**Note**: this feature doesn't work on IE due to its poor support for HTML5 drag & drop API.

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

### -AllowExport
It enable the export button for orgchart.

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

### -ExportFileName
It's filename when you export current orgchart as a picture.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
Default value: PSWriteHTML-OrgChart
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportExtension
Available values are png and pdf.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: Png
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChartID
Forces ChartID to be set to known value rather than having it autogenerated

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
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
