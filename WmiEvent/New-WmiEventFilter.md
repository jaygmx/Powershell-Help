---
external help file: WmiEvent-Help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# New-WmiEventFilter

## SYNOPSIS

## SYNTAX

### ByComputerName
```
New-WmiEventFilter [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] -EventNamespace <String> -Query <String> -QueryLanguage <String> [<CommonParameters>]
```

### ByCimSession
```
New-WmiEventFilter -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] -EventNamespace <String>
 -Query <String> -QueryLanguage <String> [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```
Add-WmiEventFilter -FilterFile ProcessStartTrace


Path          : \\localhost\root\subscription:__EventFilter.Name="ProcessStartTrace"
RelativePath  : __EventFilter.Name="ProcessStartTrace"
Server        : localhost
NamespacePath : root\subscription
ClassName     : __EventFilter
IsClass       : False
IsInstance    : True
IsSingleton   : False
```

### EXAMPLE 2
```
Add-WMIEventFilter -Name Test -EventNamespace root\subscription -Query 'SELECT * FROM __InstanceCreationEvent WITHIN 10 WHERE TargetInstance ISA __EventFilter' -QueryLanguage WQL


Path          : \\localhost\root\subscription:__EventFilter.Name="Test"
RelativePath  : __EventFilter.Name="Test"
Server        : localhost
NamespacePath : root\subscription
ClassName     : __EventFilter
IsClass       : False
IsInstance    : True
IsSingleton   : False
```

## PARAMETERS

### -ComputerName
Adds an Event Filter running on the specified computers.
The default is the local computer.

Type the NetBIOS name, an IP address, or a fully qualified domain name of one or more computers.
To specify the local computer, type the computer name, a dot (.), or "localhost".

This parameter does not rely on Windows PowerShell remoting.
You can use the ComputerName parameter of Add-WmiEventFilter even if your computer is not configured to run remote commands.

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
Unique identifier of an event filter.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EventNamespace
Namespace of the event instance used for cross-namespace subscriptions.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: Root\cimv2
Accept pipeline input: False
Accept wildcard characters: False
```

### -Query
Windows Management Instrumentation Query Language (WQL) event query that specifies the set of events for consumer notification, and the specific conditions for notification.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -QueryLanguage
Language used for the query.
Because WMI currently supports only WMI Query Language (WQL) as a query language, this property must be set to "WQL".

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: WQL
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
