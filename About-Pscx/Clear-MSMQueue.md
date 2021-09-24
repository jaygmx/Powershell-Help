---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Clear-MSMQueue

## SYNOPSIS
PSCX Cmdlet: Purges all messages from a queue

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Clear-MSMQueue [-Path <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Clear-MSMQueue [[-Name] <String>] [-MachineName <String>] [-Private] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Clear-MSMQueue [-Queue <MessageQueueInfo>] [<CommonParameters>]
```

## DESCRIPTION
Purges all messages from a queue

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS
