---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# New-UDEndpointSchedule

## SYNOPSIS
Creates a schedule for an endpoint.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDEndpointSchedule [-Consecutive] [-Cron <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDEndpointSchedule [-Consecutive] [-Day] -Every <Int32> [-Repeat <Int32>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
New-UDEndpointSchedule [-Consecutive] -Every <Int32> [-Repeat <Int32>] [-Second] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_4
```
New-UDEndpointSchedule [-Consecutive] -Every <Int32> [-Minute] [-Repeat <Int32>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_5
```
New-UDEndpointSchedule [-Consecutive] -Every <Int32> [-Hour] [-Repeat <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Creates a schedule for an endpoint.

## EXAMPLES

### Example 1
```
PS C:\> $EndpointSchedule = New-UDEndpointSchedule -Every 10 -Second
PS C:\> $Endpoint = New-UDEndpoint -Schedule $Schedule -Endpoint {
    $Cache:Computers = Get-ADComputer
}
```

Gets a list of computers from Active Directory and stores it in the cache every ten seconds.

### Example 2
```
PS C:\> $EndpointSchedule = New-UDEndpointSchedule -Every 10 -Second -Consecutive
PS C:\> $Endpoint = New-UDEndpoint -Schedule $Schedule -Endpoint {
    $Cache:Date = Get-Date
	Start-Sleep -Seconds 21
}
```

Gets the current date every 30 seconds.

### Example 3
```
PS C:\> $EndpointSchedule = New-UDEndpointSchedule -Every 10 -Second -Consecutive -Repeat 10
PS C:\> $Endpoint = New-UDEndpoint -Schedule $Schedule -Endpoint {
    $Cache:Date = Get-Date
	Start-Sleep -Seconds 21
}
```

Gets the current date every 30 seconds 10 times.

## PARAMETERS

### -Consecutive
Disables concurrently running this schedule.
Ie, it does not allow the schedule to run multiple instances.

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

### -Cron
A CRON expression to run the schedule under.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Day
Switches the Every value to days.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Every
Number of time units.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Hour
Switches the Every value to hours.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_5
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Minute
Switches the Every value to minutes.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Repeat
If set to 0 this means repeat forever, if not set it will also repeat forever.
Otherwise it will run the schedule x amount of times.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4, UNNAMED_PARAMETER_SET_5
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Second
Switches the Every value to seconds.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: True
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
