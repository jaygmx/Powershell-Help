---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcSqlSettingConfig

## SYNOPSIS


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


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -BackupConfigEnabled


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
