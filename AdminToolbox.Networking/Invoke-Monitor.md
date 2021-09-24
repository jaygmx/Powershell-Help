---
external help file: AdminToolbox.Networking-help.xml
Module Name: AdminToolbox.Networking
online version:
schema: 2.0.0
---

# Invoke-Monitor

## SYNOPSIS

## SYNTAX

```
Invoke-Monitor [-Service] <Object> [-Port] <Object> [<CommonParameters>]
```

## DESCRIPTION
Monitor a down service until it is reachable.
Provides time elapsed for the monitor and an audible indication when the services is back online.

## EXAMPLES

### EXAMPLE 1
```
Invoke-Monitor -Service Microsoft.com -port 443
```

## PARAMETERS

### -Service
Specify the service to monitor

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Port
Specify the port to monitor

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Requires the Admintoolbox.Fun module

## RELATED LINKS

[Get-Emote
Test-Netconnection]()

