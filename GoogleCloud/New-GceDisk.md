---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GceDisk

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### EmptyDisk (Default)
```
New-GceDisk [-Project <String>] [-Zone <String>] [-DiskName] <String> [-Description <String>] [-SizeGb <Int64>]
 [-DiskType <String>] [-Label <Hashtable>] [<CommonParameters>]
```

### FromImage
```
New-GceDisk [-Project <String>] [-Zone <String>] [-DiskName] <String> [-Description <String>] [-SizeGb <Int64>]
 [-DiskType <String>] [-Label <Hashtable>] [-Image] <Image> [<CommonParameters>]
```

### FromSnapshot
```
New-GceDisk [-Project <String>] [-Zone <String>] [-DiskName] <String> [-Description <String>] [-SizeGb <Int64>]
 [-DiskType <String>] [-Label <Hashtable>] [-Snapshot] <Snapshot> [<CommonParameters>]
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

### -Description
{{ Fill Description Description }}

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

### -DiskName
{{ Fill DiskName Description }}

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

### -DiskType
{{ Fill DiskType Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: pd-ssd, pd-standard

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Image
{{ Fill Image Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.Image
Parameter Sets: FromImage
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Label
{{ Fill Label Description }}

```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
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

### -SizeGb
{{ Fill SizeGb Description }}

```yaml
Type: System.Nullable`1[System.Int64]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Snapshot
{{ Fill Snapshot Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.Snapshot
Parameter Sets: FromSnapshot
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
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

### Google.Apis.Compute.v1.Data.Image

### Google.Apis.Compute.v1.Data.Snapshot

## OUTPUTS

### Google.Apis.Compute.v1.Data.Disk

## NOTES

## RELATED LINKS
