---
external help file: WmiEvent-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# New-WmiEventFilter

## SYNOPSIS

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-WmiEventFilter [-ComputerName <String[]>] -Name <String> [-EventNamespace <String>] -Query <String>
 [-QueryLanguage <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-WmiEventFilter [-ComputerName <String[]>] -FilterFile <String> [<CommonParameters>]
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
Unique identifier of an event filter.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
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
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: Root\cimv2
Accept pipeline input: False
Accept wildcard characters: False
```

### -Query
Windows Management Instrumentation Query Language (WQL) event query that specifies the set of events for consumer notification, and the specific conditions for notification.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
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
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: WQL
Accept pipeline input: False
Accept wildcard characters: False
```

### -FilterFile
The name of a filter definition file (contained within $ModulePath\Filters) without the file extension.

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
