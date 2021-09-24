---
external help file: WmiEvent-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# New-WmiEventBinding

## SYNOPSIS

## SYNTAX

```
New-WmiEventBinding [-ComputerName <String[]>] -FilterName <String> -ConsumerName <String> [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```
PS C:\> Add-WmiEventSubscription -FilterName ProcessStartTrace -ConsumerName AS_ExtrinsicHTTPPOST


Path          : \\localhost\root\subscription:__FilterToConsumerBinding.Consumer="\\\\WIN-OL5AKAF1OUJ\\ROOT\\subscripti
                on:ActiveScriptEventConsumer.Name=\"AS_ExtrinsicHTTPPOST\"",Filter="\\\\WIN-OL5AKAF1OUJ\\ROOT\\subscrip
                tion:__EventFilter.Name=\"ProcessStartTrace\""
RelativePath  : __FilterToConsumerBinding.Consumer="\\\\WIN-OL5AKAF1OUJ\\ROOT\\subscription:ActiveScriptEventConsumer.N
                ame=\"AS_ExtrinsicHTTPPOST\"",Filter="\\\\WIN-OL5AKAF1OUJ\\ROOT\\subscription:__EventFilter.Name=\"Proc
                essStartTrace\""
Server        : localhost
NamespacePath : root\subscription
ClassName     : __FilterToConsumerBinding
IsClass       : False
IsInstance    : True
IsSingleton   : False
```

Adds an Event Subscription binding the ProcessStartTrace filter with the AS_ExtrinsicHTTPPOST consumer.

## PARAMETERS

### -ComputerName
Adds an Event Subscription running on the specified computers.
The default is the local computer.

Type the NetBIOS name, an IP address, or a fully qualified domain name of one or more computers.
To specify the local computer, type the computer name, a dot (.), or "localhost".

This parameter does not rely on Windows PowerShell remoting.
You can use the ComputerName parameter of Add-WmiEventSubscription even if your computer is not configured to run remote commands.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -FilterName
Name of the Filter to use for subscription.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConsumerName
Name of the Consumer to use for subscription.

```yaml
Type: String
Parameter Sets: (All)
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
