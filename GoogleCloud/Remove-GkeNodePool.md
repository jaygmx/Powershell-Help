---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Remove-GkeNodePool

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByClusterName
```
Remove-GkeNodePool [-Project <String>] [-Zone <String>] [-NodePoolName] <String> [-ClusterName] <String>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByClusterObject
```
Remove-GkeNodePool [-NodePoolName] <String> [-ClusterObject] <Cluster> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ByNodePoolObject
```
Remove-GkeNodePool -NodePoolObject <NodePool> [-WhatIf] [-Confirm] [<CommonParameters>]
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

### -ClusterName
{{ Fill ClusterName Description }}

```yaml
Type: System.String
Parameter Sets: ByClusterName
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClusterObject
{{ Fill ClusterObject Description }}

```yaml
Type: Google.Apis.Container.v1.Data.Cluster
Parameter Sets: ByClusterObject
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NodePoolName
{{ Fill NodePoolName Description }}

```yaml
Type: System.String
Parameter Sets: ByClusterName, ByClusterObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NodePoolObject
{{ Fill NodePoolObject Description }}

```yaml
Type: Google.Apis.Container.v1.Data.NodePool
Parameter Sets: ByNodePoolObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Project
{{ Fill Project Description }}

```yaml
Type: System.String
Parameter Sets: ByClusterName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Zone
{{ Fill Zone Description }}

```yaml
Type: System.String
Parameter Sets: ByClusterName
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

### None

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
