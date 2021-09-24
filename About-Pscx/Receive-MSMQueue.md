---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Receive-MSMQueue

## SYNOPSIS
PSCX Cmdlet: Receives the first message available in the queue.
This call is synchronous, and blocks the current thread of execution until a message is available.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Receive-MSMQueue [-Formatter <IMessageFormatter>] [-Path <String>] [-Peek] [-TargetType <Type>]
 [-Timeout <TimeSpan>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Receive-MSMQueue [[-Name] <String>] [-Formatter <IMessageFormatter>] [-MachineName <String>] [-Peek] [-Private]
 [-TargetType <Type>] [-Timeout <TimeSpan>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Receive-MSMQueue [-Formatter <IMessageFormatter>] [-Peek] [-Queue <MessageQueueInfo>] [-TargetType <Type>]
 [-Timeout <TimeSpan>] [<CommonParameters>]
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
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

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
Type: IMessageFormatter
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
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
The queue's path

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
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
Type: SwitchParameter
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
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
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
Type: MessageQueueInfo
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

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
Type: Type
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
Type: TimeSpan
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

## OUTPUTS

### An object deserialized from the body of the message.
## NOTES
*

## RELATED LINKS
