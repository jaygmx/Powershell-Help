---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcLogEntry

## SYNOPSIS
{{ Fill in the Synopsis }}

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
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -JsonPayload
{{ Fill JsonPayload Description }}

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
{{ Fill LogName Description }}

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
{{ Fill MonitoredResource Description }}

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

### -ProtoPayload
{{ Fill ProtoPayload Description }}

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
{{ Fill Severity Description }}

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
{{ Fill TextPayload Description }}

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
