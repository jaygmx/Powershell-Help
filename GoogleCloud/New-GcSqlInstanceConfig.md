---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcSqlInstanceConfig

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
New-GcSqlInstanceConfig [-Project <String>] [-Name] <String> -SettingConfig <Settings> [-DatabaseVer <String>]
 [-MasterInstanceName <String>] [-FailoverReplica <String>] [-ReplicaConfig <ReplicaConfiguration>]
 [-Region <String>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -DatabaseVer
{{ Fill DatabaseVer Description }}

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

### -FailoverReplica
{{ Fill FailoverReplica Description }}

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

### -MasterInstanceName
{{ Fill MasterInstanceName Description }}

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

### -Name
{{ Fill Name Description }}

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

### -Region
{{ Fill Region Description }}

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

### -ReplicaConfig
{{ Fill ReplicaConfig Description }}

```yaml
Type: Google.Apis.SQLAdmin.v1beta4.Data.ReplicaConfiguration
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SettingConfig
{{ Fill SettingConfig Description }}

```yaml
Type: Google.Apis.SQLAdmin.v1beta4.Data.Settings
Parameter Sets: (All)
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

### Google.Apis.SQLAdmin.v1beta4.Data.Settings

### Google.Apis.SQLAdmin.v1beta4.Data.ReplicaConfiguration

## OUTPUTS

### Google.Apis.SQLAdmin.v1beta4.Data.DatabaseInstance

## NOTES

## RELATED LINKS
