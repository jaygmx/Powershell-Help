---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Clear-MSMQueue

## SYNOPSIS
PSCX Cmdlet: Purges all messages from a queue

## SYNTAX

### Named (Default)
```
Clear-MSMQueue [-MachineName <String>] [[-Name] <String>] [-Private] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Path
```
Clear-MSMQueue [-Path <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Queue
```
Clear-MSMQueue [-Queue <MessageQueueInfo>] [-WhatIf] [-Confirm] [<CommonParameters>]
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
Type: System.String
Parameter Sets: Named
Aliases: QueueName, qn

Required: False
Position: 1
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

## NOTES

## RELATED LINKS
