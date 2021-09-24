---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/tricks/network/ping
schema: 2.0.0
---

# Test-PSOnePing

## SYNOPSIS
Sends a ping (ICMP) to a computer

## SYNTAX

```
Test-PSOnePing [-ComputerName] <String[]> [[-Timeout] <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Sends a ping (ICMP) to a computer

## EXAMPLES

### EXAMPLE 1
```
Test-PSOnePing -ComputerName 127.0.0.1, microsoft.com, powershell.one -Timeout 2000
Pings three computers with a maximum timeout of 2000 milliseconds
```

### EXAMPLE 2
```
'127.0.0.1', 'microsoft.com', 'powershell.one' | Test-PSOnePing -Timeout 2000 
Pings three computers with a maximum timeout of 2000 milliseconds
```

### EXAMPLE 3
```
Get-ADComputer -Filter * | Select-Object -ExpandProperty Name | Test-PSOnePing -Timeout 2000
Pings all computers received from Get-ADComputer with a maximum timeout of 2000 milliseconds
Module "ActiveDirectory" required for Get-ADComputer
```

## PARAMETERS

### -ComputerName
Computername or IP address to ping

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Timeout
Timeout in milliseconds

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: 2000
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one/tricks/network/ping](https://powershell.one/tricks/network/ping)

