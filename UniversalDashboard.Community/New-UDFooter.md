---
external help file: UniversalDashboard.dll-Help.xml
Module Name: UniversalDashboard.Community
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# New-UDFooter

## SYNOPSIS
Configuration options for the footer.

## SYNTAX

```
New-UDFooter [-Links <Hashtable[]>] [-Copyright <String>] [-BackgroundColor <DashboardColor>]
 [-FontColor <DashboardColor>] [-Endpoint <ScriptBlock>] [-ArgumentList <Object[]>] [-AutoRefresh]
 [-RefreshInterval <Int32>] [-Id <String>] [<CommonParameters>]
```

## DESCRIPTION
Configuration options for the footer.
The options can be passed to the -Footer parameter of New-UDDashboard.

## EXAMPLES

### Example 1
```
PS C:\> $footer = New-UDFooter -Copyright "Copyright Ironman Software, LLC"
PS C:\> $dashboard = New-UDDashboard -Footer $footer
```

Sets the copyright text of the dashboard footer.

## PARAMETERS

### -ArgumentList
Arguments to pass to the endpoint.
They will be available via the $ArgumentList variable.

```yaml
Type: System.Object[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutoRefresh
Not used

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

### -BackgroundColor
Background color of the footer.
If not specified, will use the NavBarBackgrondColor set on New-UDDashboard.

```yaml
Type: UniversalDashboard.Models.DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Copyright
Copyright text.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Endpoint
Not used

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontColor
Font color of the footer.
If not specified, will use the NavBarFontColor set on New-UDDashboard.

```yaml
Type: UniversalDashboard.Models.DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Not used

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Links
Links to display in the footer.
Use New-UDLink to generate a link.

```yaml
Type: System.Collections.Hashtable[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RefreshInterval
Not used

```yaml
Type: System.Int32
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

## RELATED LINKS
