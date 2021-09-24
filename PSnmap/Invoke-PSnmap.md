---
external help file: PSnmap-help.xml
Module Name: PSNmap
online version:
schema: 2.0.0
---

# Invoke-PSnmap

## SYNOPSIS
Linux nmap for PowerShell (almost).
Ping sweeps and scans a network for specified open ports.
Can also perform DNS lookups.
Port connect timeout is custom (milliseconds).
Multithreaded with a default of 32 concurrent threads.

If you get over about 20-25,000 threads, you'll experience significant slowdowns
towards the end, so avoiding that is recommended.
This number may vary in your environment.

Svendsen Tech.
Copyright (c) 2015, Joakim Borger Svendsen.
All rights reserved.

MIT license.
http://www.opensource.org/licenses/MIT

Homepage/documentation:
https://www.powershelladmin.com/wiki/Port_scan_subnets_with_PSnmap_for_PowerShell

## SYNTAX

```
Invoke-PSnmap [-ComputerName] <String[]> [[-Port] <Int32[]>] [-Dns] [-ScanOnPingFail]
 [[-ThrottleLimit] <Int32>] [-HideProgress] [[-Timeout] <Int32>] [[-PortConnectTimeoutMs] <Int32>] [-NoSummary]
 [-AddService] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### EXAMPLE 1
```
$x = PSnmap -Cn 192.168.1.1/24, synology, ubuntuvm, vista64esxi -Port 22,3389,80,443 -Dns #-Verbose
PS C:\> $x | Where { $_.Ping } | Format-Table -AutoSize
```

ComputerName  IP/DNS                                    Ping Port 22 Port 80 Port 443 Port 3389
------------  ------                                    ---- ------- ------- -------- ---------
192.168.1.1   router.asus.com                           True   False    True    False     False
192.168.1.17  Chromecast                                True   False   False    False     False
192.168.1.25  android-xxxxxxxxxxxxxxx                   True   False   False    False     False
192.168.1.31  ubuntuvm                                  True    True    True    False     False
192.168.1.77                                            True    True   False    False     False
192.168.1.84  synology                                  True    True    True     True     False
192.168.1.122 desktop                                   True   False   False    False     False
192.168.1.124 PC58271                                   True   False    True     True      True
192.168.1.127 stuepc                                    True   False   False    False      True
192.168.1.131 2008r2esxi                                True   False    True    False      True
192.168.1.132 2008r2esxi2                               True   False    True    False      True
192.168.1.133 win7esxi                                  True   False   False    False      True
192.168.1.151 SERVER2008                                True   False   False    False      True
192.168.1.166                                           True    True    True     True     False
192.168.1.195                                           True   False   False    False     False
192.168.1.231 HPENVY4500                                True   False    True     True     False
192.168.1.234 elitebook                                 True    True   False    False      True
192.168.1.245 server2012                                True   False    True    False      True
192.168.1.253 vista64esxi                               True   False   False    False      True
synology      192.168.1.84                              True    True    True     True     False
ubuntuvm      192.168.1.31                              True    True    True    False     False
vista64esxi   fa70::614c:f45a:72f9:46a5%3;192.168.1.253 True   False   False    False      True

### EXAMPLE 2
```
$x = PSnmap -Cn 192.168.1.1/24, synology, ubuntuvm, vista64esxi -Port 22,3389,80,443 -Dns #-Verbose
PS C:\> $x | Where { $_.'Port 22' } | Format-Table -AutoSize
```

ComputerName  IP/DNS       Ping Port 22 Port 80 Port 443 Port 3389
------------  ------       ---- ------- ------- -------- ---------
192.168.1.31  ubuntuvm     True    True    True    False     False
192.168.1.77               True    True   False    False     False
192.168.1.84  synology     True    True    True     True     False
192.168.1.166              True    True    True     True     False
192.168.1.234 elitebook    True    True   False    False      True
synology      192.168.1.84 True    True    True     True     False
ubuntuvm      192.168.1.31 True    True    True    False     False

## PARAMETERS

### -ComputerName
List of CIDR, IP/subnet, IP or DNS/NetBIOS name.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: PSComputerName, Cn

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Port
Port or ports to check.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Dns
Perform a DNS lookup.

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

### -ScanOnPingFail
Scan all hosts even if ping fails.

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

### -ThrottleLimit
Number of concurrent threads.
Default: 32.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 32
Accept pipeline input: False
Accept wildcard characters: False
```

### -HideProgress
Do not display progress with Write-Progress

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

### -Timeout
Timeout in seconds for each thread.
Causes problems if too short.
30 as a default seems OK.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 30
Accept pipeline input: False
Accept wildcard characters: False
```

### -PortConnectTimeoutMs
Port connect timeout in milliseconds.
5 seconds as a default for LAN scans.
Increase for mobile/slow WAN.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: 5000
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoSummary
Do not display the end summary with start and end time, using Write-Host.

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

### -AddService
Add IANA service for the port number in parentheses.

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
