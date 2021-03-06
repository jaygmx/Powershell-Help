---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Send-GcpsAck

## SYNOPSIS


## SYNTAX

### ByName
```
Send-GcpsAck [-Project <String>] [-Subscription] <String> -AckId <String[]> [<CommonParameters>]
```

### ByObject
```
Send-GcpsAck -InputObject <PubSubMessageWithAckIdAndSubscription[]> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -AckId


```yaml
Type: System.String[]
Parameter Sets: ByName
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InputObject


```yaml
Type: Google.PowerShell.PubSub.PubSubMessageWithAckIdAndSubscription[]
Parameter Sets: ByObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Project


```yaml
Type: System.String
Parameter Sets: ByName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subscription


```yaml
Type: System.String
Parameter Sets: ByName
Aliases: Name

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String[]

### Google.PowerShell.PubSub.PubSubMessageWithAckIdAndSubscription[]

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
