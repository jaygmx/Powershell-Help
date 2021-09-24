---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceInstanceTemplate

## SYNOPSIS
{{ Fill in the Synopsis }}

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
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -AutomaticRestart
{{ Fill AutomaticRestart Description }}

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
{{ Fill BootDiskImage Description }}

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
{{ Fill CanIpForward Description }}

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
{{ Fill CustomCpu Description }}

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
{{ Fill CustomMemory Description }}

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
{{ Fill Description Description }}

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
{{ Fill Disk Description }}

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
{{ Fill ExtraDisk Description }}

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
{{ Fill Label Description }}

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
{{ Fill MachineType Description }}

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
{{ Fill Metadata Description }}

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
{{ Fill Name Description }}

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
{{ Fill Network Description }}

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
{{ Fill NoExternalIp Description }}

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
{{ Fill Object Description }}

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
{{ Fill Preemptible Description }}

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
Parameter Sets: ByValues, ByValuesCustomMachine
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceAccount
{{ Fill ServiceAccount Description }}

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
{{ Fill Subnetwork Description }}

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
{{ Fill Tag Description }}

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
{{ Fill TerminateOnMaintenance Description }}

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
