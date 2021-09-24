---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# Stop-UDRestApi

## SYNOPSIS
Stops a REST API server.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Stop-UDRestApi [-Name] <String> [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Stop-UDRestApi [-Server] <Server> [<CommonParameters>]
```

## DESCRIPTION
Stops a REST API server started with Start-UDRestApi

## EXAMPLES

### Example 1
```
PS C:\> Get-UDRestApi | Stop-UDRestApi
```

Stops all running REST API servers.

## PARAMETERS

### -Name
The name of the REST API server to stop.

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

### -Server
The server object to stop.
This is returned by Get-UDRestApi and Start-UDRestApi.

```yaml
Type: Server
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

### UniversalDashboard.Server
## OUTPUTS

### System.Object
## NOTES
*

## RELATED LINKS
