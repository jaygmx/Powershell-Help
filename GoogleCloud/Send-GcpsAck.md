---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Send-GcpsAck

## SYNOPSIS
{{ Fill in the Synopsis }}

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
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -AckId
{{ Fill AckId Description }}

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
{{ Fill InputObject Description }}

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
{{ Fill Project Description }}

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
{{ Fill Subscription Description }}

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
