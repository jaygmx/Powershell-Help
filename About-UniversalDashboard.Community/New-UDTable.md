---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDTable.md
schema: 2.0.0
---

# New-UDTable

## SYNOPSIS
Creates a new table of data within the dashboard.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDTable [-ArgumentList <Object[]>] [-AutoRefresh] [-BackgroundColor <DashboardColor>] -Endpoint <Object>
 [-FontColor <DashboardColor>] -Headers <String[]> [-Id <String>] [-Links <Hashtable[]>]
 [-RefreshInterval <Int32>] [-Style <String>] [-Title <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDTable [-ArgumentList <Object[]>] [-BackgroundColor <DashboardColor>] [-Content <ScriptBlock>]
 [-FontColor <DashboardColor>] -Headers <String[]> [-Id <String>] [-Links <Hashtable[]>] [-Style <String>]
 [-Title <String>] [<CommonParameters>]
```

## DESCRIPTION
Creates a new table of data within the dashboard.

## EXAMPLES

### Example 1
```
New-UDTable -Title "Process Ids" -Header @("Name", "Process Id") -Endpoint {
    $Data = @(
        [PSCustomObject]@{ name = "Chrome"; id = 12352 }
        [PSCustomObject]@{ name = "devenv"; id = 342 }
        [PSCustomObject]@{ name = "code"; id = 634532 }
        [PSCustomObject]@{ name = "powershell_ise"; id = 345342 }
    )
    $Data | Out-UDTableData -Property @("name", "id")
}
```

Creates a new table with the process IDs of chrome running on the system.

## PARAMETERS

### -ArgumentList
Pass arguments to Endpoints.

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutoRefresh
Enabled auto refresh for this control.

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
Background color of the table.

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
Static content for this table.

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
The endpoint to call to retrieve data for the table.
The endpoint should return data using the Out-UDTableData cmdlet.

```yaml
Type: Object
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontColor
Font color within the table.

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

### -Headers
Headers for columns in the table.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The ID of the table.
This is the HTML markup ID.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Links
Links to display on the bottom of the table.
Use New-UDLink to generate a link.

```yaml
Type: Hashtable[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RefreshInterval
The number of seconds between refreshes.
The default is 5.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Style
Allows for changing the style of the table.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Accepted values: bordered, striped, highlight, centered, responsive-table

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Title
Title for the section containing the table.

```yaml
Type: String
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

### None
## OUTPUTS

### System.Object
## NOTES
*

## RELATED LINKS
