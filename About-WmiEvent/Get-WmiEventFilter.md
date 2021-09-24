---
external help file: WmiEvent-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-WmiEventFilter

## SYNOPSIS

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-WmiEventFilter [-ComputerName <String[]>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-WmiEventFilter [-ComputerName <String[]>] -Name <String> [<CommonParameters>]
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
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Localhost
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Unique identifier of an event filter to Get.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
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
