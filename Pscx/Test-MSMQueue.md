---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Test-MSMQueue

## SYNOPSIS
PSCX Cmdlet:

## SYNTAX

### Named (Default)
```
Test-MSMQueue [-MachineName <String>] [[-Name] <String>] [-Private] [<CommonParameters>]
```

### Path
```
Test-MSMQueue [-Path <String>] [<CommonParameters>]
```

### Queue
```
Test-MSMQueue [-Queue <MessageQueueInfo>] [<CommonParameters>]
```

## DESCRIPTION

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
@{Text=}

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
@{Text=}

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
@{Text=}

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
@{Text=}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
