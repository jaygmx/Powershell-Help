---
external help file: WmiEvent-help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# New-WmiEventSubscription

## SYNOPSIS


## SYNTAX

### ComputerByValueSet
```
New-WmiEventSubscription [-ComputerName <String[]>] [-Credential <PSCredential>] -Consumer <CimInstance>
 -Filter <CimInstance> [<CommonParameters>]
```

### ComputerByNameSet
```
New-WmiEventSubscription [-ComputerName <String[]>] [-Credential <PSCredential>] -FilterName <String>
 -ConsumerType <String> -ConsumerName <String> [<CommonParameters>]
```

### SessionByValueSet
```
New-WmiEventSubscription -CimSession <CimSession[]> -Consumer <CimInstance> -Filter <CimInstance>
 [<CommonParameters>]
```

### SessionByNameSet
```
New-WmiEventSubscription -CimSession <CimSession[]> -FilterName <String> -ConsumerType <String>
 -ConsumerName <String> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -CimSession


```yaml
Type: Microsoft.Management.Infrastructure.CimSession[]
Parameter Sets: SessionByValueSet, SessionByNameSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComputerName


```yaml
Type: System.String[]
Parameter Sets: ComputerByValueSet, ComputerByNameSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Consumer


```yaml
Type: Microsoft.Management.Infrastructure.CimInstance
Parameter Sets: ComputerByValueSet, SessionByValueSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConsumerName


```yaml
Type: System.String
Parameter Sets: ComputerByNameSet, SessionByNameSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConsumerType


```yaml
Type: System.String
Parameter Sets: ComputerByNameSet, SessionByNameSet
Aliases:
Accepted values: ActiveScriptEventConsumer, CommandLineEventConsumer, LogFileEventConsumer, NtEventLogEventConsumer, SMTPEventConsumer

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential


```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: ComputerByValueSet, ComputerByNameSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filter


```yaml
Type: Microsoft.Management.Infrastructure.CimInstance
Parameter Sets: ComputerByValueSet, SessionByValueSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FilterName


```yaml
Type: System.String
Parameter Sets: ComputerByNameSet, SessionByNameSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
