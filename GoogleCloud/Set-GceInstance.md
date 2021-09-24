---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Set-GceInstance

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### AccessConfig
```
Set-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> -NetworkInterface <String>
 [-AddAccessConfig <AccessConfig[]>] [-RemoveAccessConfig <String[]>] [<CommonParameters>]
```

### Disk
```
Set-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> [-AddDisk <Object[]>]
 [-RemoveDisk <String[]>] [<CommonParameters>]
```

### AutoDeleteDisk
```
Set-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> [-TurnOnAutoDeleteDisk <String[]>]
 [-TurnOffAutoDeleteDisk <String[]>] [<CommonParameters>]
```

### Metadata
```
Set-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> [-AddMetadata <Hashtable>]
 [-RemoveMetadata <String[]>] [<CommonParameters>]
```

### Tag
```
Set-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> [-AddTag <String[]>]
 [-RemoveTag <String[]>] [<CommonParameters>]
```

### AccessConfigByObject
```
Set-GceInstance [-Object] <Instance> -NetworkInterface <String> [-AddAccessConfig <AccessConfig[]>]
 [-RemoveAccessConfig <String[]>] [<CommonParameters>]
```

### DiskByObject
```
Set-GceInstance [-Object] <Instance> [-AddDisk <Object[]>] [-RemoveDisk <String[]>] [<CommonParameters>]
```

### AutoDeleteDiskByObject
```
Set-GceInstance [-Object] <Instance> [-TurnOnAutoDeleteDisk <String[]>] [-TurnOffAutoDeleteDisk <String[]>]
 [<CommonParameters>]
```

### MetadataByObject
```
Set-GceInstance [-Object] <Instance> [-AddMetadata <Hashtable>] [-RemoveMetadata <String[]>]
 [<CommonParameters>]
```

### TagByObject
```
Set-GceInstance [-Object] <Instance> [-AddTag <String[]>] [-RemoveTag <String[]>] [<CommonParameters>]
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

### -AddAccessConfig
{{ Fill AddAccessConfig Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.AccessConfig[]
Parameter Sets: AccessConfig, AccessConfigByObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AddDisk
{{ Fill AddDisk Description }}

```yaml
Type: System.Object[]
Parameter Sets: Disk, DiskByObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AddMetadata
{{ Fill AddMetadata Description }}

```yaml
Type: System.Collections.Hashtable
Parameter Sets: Metadata, MetadataByObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AddTag
{{ Fill AddTag Description }}

```yaml
Type: System.String[]
Parameter Sets: Tag, TagByObject
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
Parameter Sets: AccessConfig, Disk, AutoDeleteDisk, Metadata, Tag
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NetworkInterface
{{ Fill NetworkInterface Description }}

```yaml
Type: System.String
Parameter Sets: AccessConfig, AccessConfigByObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Object
{{ Fill Object Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.Instance
Parameter Sets: AccessConfigByObject, DiskByObject, AutoDeleteDiskByObject, MetadataByObject, TagByObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Project
{{ Fill Project Description }}

```yaml
Type: System.String
Parameter Sets: AccessConfig, Disk, AutoDeleteDisk, Metadata, Tag
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveAccessConfig
{{ Fill RemoveAccessConfig Description }}

```yaml
Type: System.String[]
Parameter Sets: AccessConfig, AccessConfigByObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveDisk
{{ Fill RemoveDisk Description }}

```yaml
Type: System.String[]
Parameter Sets: Disk, DiskByObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveMetadata
{{ Fill RemoveMetadata Description }}

```yaml
Type: System.String[]
Parameter Sets: Metadata, MetadataByObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveTag
{{ Fill RemoveTag Description }}

```yaml
Type: System.String[]
Parameter Sets: Tag, TagByObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TurnOffAutoDeleteDisk
{{ Fill TurnOffAutoDeleteDisk Description }}

```yaml
Type: System.String[]
Parameter Sets: AutoDeleteDisk, AutoDeleteDiskByObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TurnOnAutoDeleteDisk
{{ Fill TurnOnAutoDeleteDisk Description }}

```yaml
Type: System.String[]
Parameter Sets: AutoDeleteDisk, AutoDeleteDiskByObject
Aliases:

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
Parameter Sets: AccessConfig, Disk, AutoDeleteDisk, Metadata, Tag
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

### Google.Apis.Compute.v1.Data.Instance

## OUTPUTS

### Google.Apis.Compute.v1.Data.Instance

## NOTES

## RELATED LINKS
