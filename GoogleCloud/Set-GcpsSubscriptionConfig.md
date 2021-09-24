---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Set-GcpsSubscriptionConfig

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### PushConfig
```
Set-GcpsSubscriptionConfig [-Project <String>] [-Subscription] <String> [-PushEndpoint] <String>
 [<CommonParameters>]
```

### PullConfig
```
Set-GcpsSubscriptionConfig [-Project <String>] [-Subscription] <String> [-PullConfig] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Project
{{ Fill Project Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PullConfig
{{ Fill PullConfig Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: PullConfig
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PushEndpoint
{{ Fill PushEndpoint Description }}

```yaml
Type: System.String
Parameter Sets: PushConfig
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subscription
{{ Fill Subscription Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
