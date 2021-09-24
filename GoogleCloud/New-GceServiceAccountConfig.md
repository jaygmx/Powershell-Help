---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GceServiceAccountConfig

## SYNOPSIS
{{ Fill in the Synopsis }}

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
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -BigQuery
{{ Fill BigQuery Description }}

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
{{ Fill BigtableAdmin Description }}

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
{{ Fill BigtableData Description }}

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
{{ Fill CloudDatastore Description }}

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
{{ Fill CloudLogging Description }}

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
{{ Fill CloudMonitoring Description }}

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
{{ Fill CloudPubSub Description }}

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
{{ Fill CloudSQL Description }}

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
{{ Fill Compute Description }}

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
{{ Fill Email Description }}

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

### -ScopeUri
{{ Fill ScopeUri Description }}

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
{{ Fill ServiceControl Description }}

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
{{ Fill ServiceManagement Description }}

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
{{ Fill Storage Description }}

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
{{ Fill TaskQueue Description }}

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
{{ Fill UserInfo Description }}

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
