---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# New-MSMQueue

## SYNOPSIS
PSCX Cmdlet: Creates a new queue object with the defined properties

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-MSMQueue [-Force] [-Path <String>] [-Transactional] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-MSMQueue [[-Name] <String>] [-Force] [-MachineName <String>] [-Private] [-Transactional]
 [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
New-MSMQueue [-Force] [-Queue <MessageQueueInfo>] [-Transactional] [<CommonParameters>]
```

## DESCRIPTION
Creates a new queue object with the defined properties

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

### -Force
Force the creation of the queue, even if a queue already exists with the given name

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

### -Transactional
Create a transactional queue.
If true, the queue will accept only messages sent as part of a transaction.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS
