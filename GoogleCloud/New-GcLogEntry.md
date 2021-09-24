---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcLogEntry

## SYNOPSIS


## SYNTAX

### TextPayload (Default)
```
New-GcLogEntry [-Project <String>] [-LogName] <String> -TextPayload <String[]> [-Severity <LogSeverity>]
 [-MonitoredResource <MonitoredResource>] [<CommonParameters>]
```

### JsonPayload
```
New-GcLogEntry [-Project <String>] [-LogName] <String> -JsonPayload <Hashtable[]> [-Severity <LogSeverity>]
 [-MonitoredResource <MonitoredResource>] [<CommonParameters>]
```

### ProtoPayload
```
New-GcLogEntry [-Project <String>] [-LogName] <String> -ProtoPayload <Hashtable[]> [-Severity <LogSeverity>]
 [-MonitoredResource <MonitoredResource>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -JsonPayload


```yaml
Type: System.Collections.Hashtable[]
Parameter Sets: JsonPayload
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LogName


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MonitoredResource


```yaml
Type: Google.Apis.Logging.v2.Data.MonitoredResource
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Project


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

### -ProtoPayload


```yaml
Type: System.Collections.Hashtable[]
Parameter Sets: ProtoPayload
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Severity


```yaml
Type: Google.PowerShell.Logging.GcLogCmdlet+LogSeverity
Parameter Sets: (All)
Aliases:
Accepted values: Default, Debug, Info, Notice, Warning, Error, Critical, Alert, Emergency

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextPayload


```yaml
Type: System.String[]
Parameter Sets: TextPayload
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String[]

### System.Collections.Hashtable[]

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
