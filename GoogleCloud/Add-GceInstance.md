---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceInstance

## SYNOPSIS


## SYNTAX

### ByValues (Default)
```
Add-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> [[-MachineType] <String>] [-CanIpForward]
 [-Description <String>] [-BootDisk <Disk>] [-BootDiskImage <Image>] [-ExtraDisk <Disk[]>]
 [-Disk <AttachedDisk[]>] [-Metadata <IDictionary>] [-Network <String>] [-Region <String>]
 [-Subnetwork <String>] [-NoExternalIp] [-Preemptible] [-AutomaticRestart <Boolean>] [-TerminateOnMaintenance]
 [-ServiceAccount <ServiceAccount[]>] [-Tag <String[]>] [-Label <Hashtable>] [-Address <String>]
 [<CommonParameters>]
```

### ByObject
```
Add-GceInstance [-Project <String>] [-Zone <String>] [-InstanceConfig] <Instance> [<CommonParameters>]
```

### ByValuesCustomMachine
```
Add-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> -CustomCpu <Int32> -CustomMemory <Int32>
 [-CanIpForward] [-Description <String>] [-BootDisk <Disk>] [-BootDiskImage <Image>] [-ExtraDisk <Disk[]>]
 [-Disk <AttachedDisk[]>] [-Metadata <IDictionary>] [-Network <String>] [-Region <String>]
 [-Subnetwork <String>] [-NoExternalIp] [-Preemptible] [-AutomaticRestart <Boolean>] [-TerminateOnMaintenance]
 [-ServiceAccount <ServiceAccount[]>] [-Tag <String[]>] [-Label <Hashtable>] [-Address <String>]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Address


```yaml
Type: System.String
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutomaticRestart


```yaml
Type: System.Boolean
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BootDisk


```yaml
Type: Google.Apis.Compute.v1.Data.Disk
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BootDiskImage


```yaml
Type: Google.Apis.Compute.v1.Data.Image
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases: DiskImage

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CanIpForward


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomCpu


```yaml
Type: System.Int32
Parameter Sets: ByValuesCustomMachine
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomMemory


```yaml
Type: System.Int32
Parameter Sets: ByValuesCustomMachine
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description


```yaml
Type: System.String
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Disk


```yaml
Type: Google.Apis.Compute.v1.Data.AttachedDisk[]
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExtraDisk


```yaml
Type: Google.Apis.Compute.v1.Data.Disk[]
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstanceConfig


```yaml
Type: Google.Apis.Compute.v1.Data.Instance
Parameter Sets: ByObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Label


```yaml
Type: System.Collections.Hashtable
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MachineType


```yaml
Type: System.String
Parameter Sets: ByValues
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Metadata


```yaml
Type: System.Collections.IDictionary
Parameter Sets: ByValues, ByValuesCustomMachine
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
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Network


```yaml
Type: System.String
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoExternalIp


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Preemptible


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByValues, ByValuesCustomMachine
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

### -Region


```yaml
Type: System.String
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceAccount


```yaml
Type: Google.Apis.Compute.v1.Data.ServiceAccount[]
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subnetwork


```yaml
Type: System.String
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tag


```yaml
Type: System.String[]
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TerminateOnMaintenance


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Zone


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

### Google.Apis.Compute.v1.Data.Instance

### System.String

## OUTPUTS

### Google.Apis.Compute.v1.Data.Instance

## NOTES

## RELATED LINKS
