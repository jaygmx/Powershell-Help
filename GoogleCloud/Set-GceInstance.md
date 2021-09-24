---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Set-GceInstance

## SYNOPSIS


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


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -AddAccessConfig


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
