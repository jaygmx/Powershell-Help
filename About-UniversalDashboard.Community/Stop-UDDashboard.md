---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# Stop-UDDashboard

## SYNOPSIS
Stops a dashboard returned by Start-UDDashboard.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Stop-UDDashboard [-Name] <String> [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Stop-UDDashboard [-Port] <Int32> [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Stop-UDDashboard [-Server] <Server> [<CommonParameters>]
```

## DESCRIPTION
Stops a dashboard returned by Start-UDDashboard.

## EXAMPLES

### Example 1
```
PS C:\> $DashboardServer = Start-UDDashboard -Content { New-UDDashboard {} }
PS C:\> Stop-UDDashboard -Server $DashboardServer
```

Stops a dashboard returned by Start-UDDashboard.

### Example 2
```
PS C:\> Stop-UDDashboard -Name "MyDashboard"
```

Stops the dashboard named "MyDashboard".

## PARAMETERS

### -Name
Name of the dashboard to stop.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Port
Stops the dashboard by port number.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Server
The dashboard server to stop.
This is returned by Start-UDDashboard.

```yaml
Type: Server
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
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
