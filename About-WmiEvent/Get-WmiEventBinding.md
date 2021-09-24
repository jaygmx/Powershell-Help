---
external help file: WmiEvent-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-WmiEventBinding

## SYNOPSIS

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-WmiEventBinding [-ComputerName <String[]>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-WmiEventBinding [-ComputerName <String[]>] [-Name <String>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```
PS C:\> Get-WmiEventSubscription

ComputerName              FilterName                ConsumerName
------------              ----------                ------------
WIN-OL5AKAF1OUJ           ProcessStartTrace         AS_ExtrinsicHTTPPOST
WIN-OL5AKAF1OUJ           ServiceCreation           AS_IntrinsicHTTPPOST
WIN-OL5AKAF1OUJ           LoggedOnUserCreation      AS_GenericHTTPPOST
```

Get all Event Subscriptions on the localhost.

### EXAMPLE 2
```
Get-WmiEventSubscription -ComputerName SERVER1

ComputerName              FilterName                ConsumerName
------------              ----------                ------------
SERVER1                   ProcessStartTrace         AS_ExtrinsicHTTPPOST
SERVER1                   ServiceCreation           AS_IntrinsicHTTPPOST
SERVER1                   LoggedOnUserCreation      AS_GenericHTTPPOST
```

Gets all Event Subscriptions on SERVER1

### EXAMPLE 3
```
Get-WmiEventSubscription -Name ProcessStartTrace

ComputerName              FilterName                ConsumerName
------------              ----------                ------------
WIN-OL5AKAF1OUJ           ProcessStartTrace         AS_ExtrinsicHTTPPOST
```

Gets the Event Subscription where the FilterName is ProcessStartTrace.

## PARAMETERS

### -ComputerName
Gets the Event Subscriptions running on the specified computers.
The default is the local computer.

Type the NetBIOS name, an IP address, or a fully qualified domain name of one or more computers.
To specify the local computer, type the computer name, a dot (.), or "localhost".

This parameter does not rely on Windows PowerShell remoting.
You can use the ComputerName parameter of Get-WmiEventSubscription even if your computer is not configured to run remote commands.

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

### -Name
@{Text=}

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
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
