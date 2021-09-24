---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/tricks/network/porttest
schema: 2.0.0
---

# Test-PSOnePort

## SYNOPSIS
Tests a network port on a remote computer

## SYNTAX

```
Test-PSOnePort [-ComputerName] <String> [-Port] <Int32> [[-Timeout] <Int32>] [[-Count] <Int32>]
 [[-Delay] <Object>] [-ExitOnSuccess] [<CommonParameters>]
```

## DESCRIPTION
Tests whether a port on a remote computer is responding.

## EXAMPLES

### EXAMPLE 1
```
Test-PSOnePort -ComputerName 127.0.0.1 -Port 4000 -Timeout 1000 
Tests whether port 4000 on the local computer is responding, 
and waits a maximum of 1000 milliseconds
```

### EXAMPLE 2
```
Test-PSOnePort -ComputerName 127.0.0.1 -Port 4000 -Timeout 1000 -Count 30 -Delay 2000
Tests 30 times whether port 4000 on the local computer is responding, 
and waits a maximum of 1000 milliseconds inbetween each test
```

### EXAMPLE 3
```
Test-PSOnePort -ComputerName 127.0.0.1 -Port 4000 -Timeout 1000 -Count 0 -Delay 2000 -ExitOnSuccess
Continuously tests whether port 4000 on the local computer is responding, 
waits a maximum of 1000 milliseconds inbetween each test, 
and exits as soon as the port is responding
```

## PARAMETERS

### -ComputerName


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Port
port number to test

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Timeout
timeout in milliseconds

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 500
Accept pipeline input: False
Accept wildcard characters: False
```

### -Count
number of tries.
A value of 0 indicates countinuous testing

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 1
Accept pipeline input: False
Accept wildcard characters: False
```

### -Delay
delay (in milliseconds) inbetween continuous tests

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: 2000
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExitOnSuccess
when enabled, function returns as soon as port is available

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one/tricks/network/porttest](https://powershell.one/tricks/network/porttest)

