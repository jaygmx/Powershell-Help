---
external help file: WmiEvent-Help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# Get-WmiEventFilter

## SYNOPSIS

## SYNTAX

### ByComputerName
```
Get-WmiEventFilter [-ComputerName <String[]>] [-Credential <PSCredential>] [-Name <String>]
 [-ThrottleLimit <Int32>] [<CommonParameters>]
```

### ByCimSession
```
Get-WmiEventFilter -CimSession <CimSession[]> [-Name <String>] [-ThrottleLimit <Int32>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```
Get-WmiEventFilter


ComputerName : WIN-OL5AKAF1OUJ
Name         : ProcessCreation
Query        : SELECT * FROM __InstanceCreationEvent WITHIN 10 WHERE TargetInstance ISA 'Win32_Process'

ComputerName : WIN-OL5AKAF1OUJ
Name         : ProcessStartTrace
Query        : SELECT * FROM Win32_ProcessStartTrace

ComputerName : WIN-OL5AKAF1OUJ
Name         : UserProfileCreation
Query        : SELECT * FROM __InstanceCreationEvent WITHIN 10 WHERE TargetInstance ISA 'Win32_UserProfile'

ComputerName : WIN-OL5AKAF1OUJ
Name         : Test
Query        : SELECT * FROM __InstanceCreationEvent WITHIN 10 WHERE TargetInstance ISA __EventFilter
```

Lists all Permanent WMI Event Filters

### EXAMPLE 2
```
Get-WmiEventFilter -ComputerName WORKSTATION1 -Name ProcessCreation


ComputerName : WIN-OL5AKAF1OUJ
Name         : ProcessCreation
Query        : SELECT * FROM __InstanceCreationEvent WITHIN 10 WHERE TargetInstance ISA 'Win32_Process'
```

Lists the Permanent WMI Event Filter name ProcessCreation on WORKSTATION1

## PARAMETERS

### -ComputerName
Gets the Event Filters running on the specified computers.
The default is the local computer.

Type the NetBIOS name, an IP address, or a fully qualified domain name of one or more computers.
To specify the local computer, type the computer name, a dot (.), or "localhost".

This parameter does not rely on Windows PowerShell remoting.
You can use the ComputerName parameter of Get-WmiEventFilter even if your computer is not configured to run remote commands.

```yaml
Type: System.String[]
Parameter Sets: ByComputerName
Aliases:

Required: False
Position: Named
Default value: Localhost
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Unique identifier of an event filter to Get.

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

### -CimSession
{{ Fill CimSession Description }}

```yaml
Type: Microsoft.Management.Infrastructure.CimSession[]
Parameter Sets: ByCimSession
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
{{ Fill Credential Description }}

```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: ByComputerName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ThrottleLimit
{{ Fill ThrottleLimit Description }}

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

### System.String[]
## OUTPUTS

## NOTES

## RELATED LINKS
