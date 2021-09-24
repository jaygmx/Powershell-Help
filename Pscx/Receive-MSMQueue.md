---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Receive-MSMQueue

## SYNOPSIS
PSCX Cmdlet: Receives the first message available in the queue.
This call is synchronous, and blocks the current thread of execution until a message is available.

## SYNTAX

### Named (Default)
```
Receive-MSMQueue [-Peek] [-TargetType <Type>] [-Timeout <TimeSpan>] [-Formatter <IMessageFormatter>]
 [-MachineName <String>] [[-Name] <String>] [-Private] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Path
```
Receive-MSMQueue [-Peek] [-TargetType <Type>] [-Timeout <TimeSpan>] [-Formatter <IMessageFormatter>]
 [-Path <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Queue
```
Receive-MSMQueue [-Peek] [-TargetType <Type>] [-Timeout <TimeSpan>] [-Formatter <IMessageFormatter>]
 [-Queue <MessageQueueInfo>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Receives the first message available in the queue.
This call is synchronous, and blocks the current thread of execution and waits until either a message is available in the queue, or the time-out expires.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Name
@{Text=}

```yaml
Type: System.String
Parameter Sets: Named
Aliases: QueueName, qn

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Formatter
The formatter used to serialize an object into or deserialize an object from the body of a message read from or written to the queue.
If supplied, TargetType property will be ignored.

```yaml
Type: System.Messaging.IMessageFormatter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MachineName
The name of the computer where the Message Queuing queue is located

```yaml
Type: System.String
Parameter Sets: Named
Aliases: ComputerName

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
The queue's path

```yaml
Type: System.String
Parameter Sets: Path
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Peek
If present, returns without removing (peeks) the first message in the queue.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Private
The visibility of the queue

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Named
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Queue
MessageQueueInfo object holding the message queue information

```yaml
Type: Pscx.Commands.Messaging.MessageQueueInfo
Parameter Sets: Queue
Aliases: QueueInfo

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TargetType
Type of object to convert the message body to, using an XMLFormatter.
If Formatter property is provided, this property will be ignored.

```yaml
Type: System.Type
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Timeout
@{Text=}

```yaml
Type: System.TimeSpan
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### An object deserialized from the body of the message.
## NOTES

## RELATED LINKS
