---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Get-GceManagedInstanceGroup

## SYNOPSIS


## SYNTAX

### ListProject (Default)
```
Get-GceManagedInstanceGroup [-Project <String>] [-InstanceStatus] [<CommonParameters>]
```

### ListZone
```
Get-GceManagedInstanceGroup [-Project <String>] -Zone <String> [-InstanceStatus] [<CommonParameters>]
```

### ListRegion
```
Get-GceManagedInstanceGroup [-Project <String>] -Region <String> [-InstanceStatus] [<CommonParameters>]
```

### ByName
```
Get-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>] [-Name] <String>
 [-InstanceStatus] [<CommonParameters>]
```

### ByUri
```
Get-GceManagedInstanceGroup -Uri <String> [-InstanceStatus] [<CommonParameters>]
```

### ByObject
```
Get-GceManagedInstanceGroup -Object <InstanceGroupManager> [-InstanceStatus] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -InstanceStatus


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

### -Name


```yaml
Type: System.String
Parameter Sets: ByName
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Object


```yaml
Type: Google.Apis.Compute.v1.Data.InstanceGroupManager
Parameter Sets: ByObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Project


```yaml
Type: System.String
Parameter Sets: ListProject, ListZone, ListRegion, ByName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Region


```yaml
Type: System.String
Parameter Sets: ListRegion
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.String
Parameter Sets: ByName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Uri


```yaml
Type: System.String
Parameter Sets: ByUri
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Zone


```yaml
Type: System.String
Parameter Sets: ListZone
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.String
Parameter Sets: ByName
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

### Google.Apis.Compute.v1.Data.InstanceGroupManager

## OUTPUTS

### Google.Apis.Compute.v1.Data.InstanceGroupManager

### Google.Apis.Compute.v1.Data.ManagedInstance

## NOTES

## RELATED LINKS
