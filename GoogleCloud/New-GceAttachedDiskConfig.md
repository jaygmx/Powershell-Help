---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GceAttachedDiskConfig

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### Persistent (Default)
```
New-GceAttachedDiskConfig [-Source] <Disk> [-AutoDelete] [-Boot] [-Nvme] [-DeviceName <String>] [-ReadOnly]
 [<CommonParameters>]
```

### New
```
New-GceAttachedDiskConfig [[-SourceImage] <Image>] [-Name <String>] [-DiskType <String>] [-Size <Int64>]
 [-AutoDelete] [-Boot] [-Nvme] [-DeviceName <String>] [-ReadOnly] [<CommonParameters>]
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

### -AutoDelete
{{ Fill AutoDelete Description }}

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

### -Boot
{{ Fill Boot Description }}

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

### -DeviceName
{{ Fill DeviceName Description }}

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

### -DiskType
{{ Fill DiskType Description }}

```yaml
Type: System.String
Parameter Sets: New
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
Parameter Sets: New
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Nvme
{{ Fill Nvme Description }}

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

### -ReadOnly
{{ Fill ReadOnly Description }}

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

### -Size
{{ Fill Size Description }}

```yaml
Type: System.Nullable`1[System.Int64]
Parameter Sets: New
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Source
{{ Fill Source Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.Disk
Parameter Sets: Persistent
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SourceImage
{{ Fill SourceImage Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.Image
Parameter Sets: New
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Compute.v1.Data.Disk

### Google.Apis.Compute.v1.Data.Image

## OUTPUTS

### Google.Apis.Compute.v1.Data.AttachedDisk

## NOTES

## RELATED LINKS
