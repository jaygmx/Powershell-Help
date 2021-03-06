---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GceServiceAccountConfig

## SYNOPSIS


## SYNTAX

### FromFlags (Default)
```
New-GceServiceAccountConfig [-Project <String>] [[-Email] <String>] [-ScopeUri <String[]>] [-BigQuery]
 [-BigtableAdmin <BigTableAdminEnum>] [-BigtableData <ReadWrite>] [-CloudDatastore] [-CloudLogging <ReadWrite>]
 [-CloudMonitoring <ReadWrite>] [-CloudPubSub] [-CloudSQL] [-Compute <ReadWrite>] [-ServiceControl <Boolean>]
 [-ServiceManagement <Boolean>] [-Storage <ReadWrite>] [-TaskQueue] [-UserInfo] [<CommonParameters>]
```

### FromScopeUris
```
New-GceServiceAccountConfig [-Project <String>] [[-Email] <String>] -ScopeUri <String[]> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -BigQuery


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BigtableAdmin


```yaml
Type: Google.PowerShell.ComputeEngine.NewGceServiceAccountConfigCmdlet+BigTableAdminEnum
Parameter Sets: FromFlags
Aliases:
Accepted values: None, Tables, Full

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BigtableData


```yaml
Type: Google.PowerShell.ComputeEngine.NewGceServiceAccountConfigCmdlet+ReadWrite
Parameter Sets: FromFlags
Aliases:
Accepted values: None, Read, ReadWrite

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloudDatastore


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloudLogging


```yaml
Type: Google.PowerShell.ComputeEngine.NewGceServiceAccountConfigCmdlet+ReadWrite
Parameter Sets: FromFlags
Aliases:
Accepted values: None, Read, Write, Full

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloudMonitoring


```yaml
Type: Google.PowerShell.ComputeEngine.NewGceServiceAccountConfigCmdlet+ReadWrite
Parameter Sets: FromFlags
Aliases:
Accepted values: None, Read, Write, Full

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloudPubSub


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloudSQL


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Compute


```yaml
Type: Google.PowerShell.ComputeEngine.NewGceServiceAccountConfigCmdlet+ReadWrite
Parameter Sets: FromFlags
Aliases:
Accepted values: None, Read, ReadWrite

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Email


```yaml
Type: System.String
Parameter Sets: FromFlags
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

```yaml
Type: System.String
Parameter Sets: FromScopeUris
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
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

### -ScopeUri


```yaml
Type: System.String[]
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.String[]
Parameter Sets: FromScopeUris
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceControl


```yaml
Type: System.Boolean
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceManagement


```yaml
Type: System.Boolean
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Storage


```yaml
Type: Google.PowerShell.ComputeEngine.NewGceServiceAccountConfigCmdlet+ReadWrite
Parameter Sets: FromFlags
Aliases:
Accepted values: None, Read, Write, ReadWrite, Full

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TaskQueue


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserInfo


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FromFlags
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

### System.String[]

## OUTPUTS

### Google.Apis.Compute.v1.Data.ServiceAccount

## NOTES

## RELATED LINKS
