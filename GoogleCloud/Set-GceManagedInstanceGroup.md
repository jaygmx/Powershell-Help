---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Set-GceManagedInstanceGroup

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### AbandonUri
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String> [-Abandon]
 -InstanceUri <String[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AbandonObject
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String> [-Abandon]
 -InstanceObject <Instance[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### DeleteUri
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String> [-Delete]
 -InstanceUri <String[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### DeleteObject
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String> [-Delete]
 -InstanceObject <Instance[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RecreateUri
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String>
 [-Recreate] -InstanceUri <String[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RecreateObject
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String>
 [-Recreate] -InstanceObject <Instance[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Resize
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String>
 -Size <Int32> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetTemplate
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String>
 -Template <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetTargetPools
```
Set-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String>
 -TargetPoolUri <String[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Abandon
{{ Fill Abandon Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: AbandonUri, AbandonObject
Aliases:

Required: True
Position: Named
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

### -Delete
{{ Fill Delete Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DeleteUri, DeleteObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstanceObject
{{ Fill InstanceObject Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.Instance[]
Parameter Sets: AbandonObject, DeleteObject, RecreateObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InstanceUri
{{ Fill InstanceUri Description }}

```yaml
Type: System.String[]
Parameter Sets: AbandonUri, DeleteUri, RecreateUri
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### -Recreate
{{ Fill Recreate Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: RecreateUri, RecreateObject
Aliases:

Required: True
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

### -Size
{{ Fill Size Description }}

```yaml
Type: System.Int32
Parameter Sets: Resize
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetPoolUri
{{ Fill TargetPoolUri Description }}

```yaml
Type: System.String[]
Parameter Sets: SetTargetPools
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Template
{{ Fill Template Description }}

```yaml
Type: System.String
Parameter Sets: SetTemplate
Aliases:

Required: True
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
Parameter Sets: (All)
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

### System.String[]

### Google.Apis.Compute.v1.Data.Instance[]

## OUTPUTS

### Google.Apis.Compute.v1.Data.InstanceGroupManager

## NOTES

## RELATED LINKS
