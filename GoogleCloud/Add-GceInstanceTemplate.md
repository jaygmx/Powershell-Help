---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceInstanceTemplate

## SYNOPSIS


## SYNTAX

### ByValues (Default)
```
Add-GceInstanceTemplate [-Project <String>] [-Name] <String> [[-MachineType] <String>] [-CanIpForward]
 [-Description <String>] [-BootDiskImage <Image>] [-ExtraDisk <Disk[]>] [-Disk <AttachedDisk[]>]
 [-Metadata <IDictionary>] [-Network <String>] [-Region <String>] [-Subnetwork <String>] [-NoExternalIp]
 [-Preemptible] [-AutomaticRestart <Boolean>] [-TerminateOnMaintenance] [-ServiceAccount <ServiceAccount[]>]
 [-Tag <String[]>] [-Label <Hashtable>] [<CommonParameters>]
```

### FromObject
```
Add-GceInstanceTemplate [-Project <String>] [-Object] <InstanceTemplate> [<CommonParameters>]
```

### ByValuesCustomMachine
```
Add-GceInstanceTemplate [-Project <String>] [-Name] <String> -CustomCpu <Int32> -CustomMemory <Int32>
 [-CanIpForward] [-Description <String>] [-BootDiskImage <Image>] [-ExtraDisk <Disk[]>]
 [-Disk <AttachedDisk[]>] [-Metadata <IDictionary>] [-Network <String>] [-Region <String>]
 [-Subnetwork <String>] [-NoExternalIp] [-Preemptible] [-AutomaticRestart <Boolean>] [-TerminateOnMaintenance]
 [-ServiceAccount <ServiceAccount[]>] [-Tag <String[]>] [-Label <Hashtable>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

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

### -BootDiskImage


```yaml
Type: Google.Apis.Compute.v1.Data.Image
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

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
Accept pipeline input: False
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

### -Object


```yaml
Type: Google.Apis.Compute.v1.Data.InstanceTemplate
Parameter Sets: FromObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Compute.v1.Data.InstanceTemplate

## OUTPUTS

### Google.Apis.Compute.v1.Data.InstanceTemplate

## NOTES

## RELATED LINKS
