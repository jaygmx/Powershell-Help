---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcSqlSettingConfig

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
New-GcSqlSettingConfig [[-TierConfig] <String>] [-Policy <ActivationPolicy>] [-BinaryLogEnabled <Boolean>]
 [-BackupConfigEnabled <Boolean>] [-BackupConfigStartTime <String>] [-DataDiskSizeGb <Int64>]
 [-DatabaseFlag <DatabaseFlags[]>] [-IpConfigAuthorizedNetwork <AclEntry[]>] [-IpConfigIpv4Enabled]
 [-IpConfigRequireSsl] [-LocationPreferenceFollowGae <String>] [-LocationPreferenceZone <String>]
 [-MaintenanceWindowDay <Int32>] [-MaintenanceWindowHour <Int32>] [-StorageAutoResize]
 [-DiskType <DataDiskType>] [<CommonParameters>]
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

### -BackupConfigEnabled
{{ Fill BackupConfigEnabled Description }}

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackupConfigStartTime
{{ Fill BackupConfigStartTime Description }}

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

### -BinaryLogEnabled
{{ Fill BinaryLogEnabled Description }}

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DataDiskSizeGb
{{ Fill DataDiskSizeGb Description }}

```yaml
Type: System.Int64
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DatabaseFlag
{{ Fill DatabaseFlag Description }}

```yaml
Type: Google.Apis.SQLAdmin.v1beta4.Data.DatabaseFlags[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DiskType
{{ Fill DiskType Description }}

```yaml
Type: Google.PowerShell.Sql.NewGcSqlSettingConfigCmdlet+DataDiskType
Parameter Sets: (All)
Aliases:
Accepted values: PD_SSD, PD_HDD

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IpConfigAuthorizedNetwork
{{ Fill IpConfigAuthorizedNetwork Description }}

```yaml
Type: Google.Apis.SQLAdmin.v1beta4.Data.AclEntry[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IpConfigIpv4Enabled
{{ Fill IpConfigIpv4Enabled Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IpConfigRequireSsl
{{ Fill IpConfigRequireSsl Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocationPreferenceFollowGae
{{ Fill LocationPreferenceFollowGae Description }}

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

### -LocationPreferenceZone
{{ Fill LocationPreferenceZone Description }}

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

### -MaintenanceWindowDay
{{ Fill MaintenanceWindowDay Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaintenanceWindowHour
{{ Fill MaintenanceWindowHour Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Policy
{{ Fill Policy Description }}

```yaml
Type: Google.PowerShell.Sql.NewGcSqlSettingConfigCmdlet+ActivationPolicy
Parameter Sets: (All)
Aliases:
Accepted values: ALWAYS, NONE

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StorageAutoResize
{{ Fill StorageAutoResize Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TierConfig
{{ Fill TierConfig Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Google.Apis.SQLAdmin.v1beta4.Data.Settings

## NOTES

## RELATED LINKS
