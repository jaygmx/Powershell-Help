---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceSnapshot

## SYNOPSIS


## SYNTAX

### FromDisk
```
Add-GceSnapshot [-Disk] <Disk> [-Label <Hashtable>] [-Name <String>] [-Description <String>] [-GuestFlush]
 [<CommonParameters>]
```

### FromDiskName
```
Add-GceSnapshot [-Project <String>] [-Zone <String>] [-Label <Hashtable>] [-DiskName] <String> [-Name <String>]
 [-Description <String>] [-GuestFlush] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Description


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

### -Disk


```yaml
Type: Google.Apis.Compute.v1.Data.Disk
Parameter Sets: FromDisk
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DiskName


```yaml
Type: System.String
Parameter Sets: FromDiskName
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GuestFlush


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: VSS

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Label


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

### -Name


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

### -Project


```yaml
Type: System.String
Parameter Sets: FromDiskName
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
Parameter Sets: FromDiskName
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

### Google.Apis.Compute.v1.Data.Disk

## OUTPUTS

### Google.Apis.Compute.v1.Data.Snapshot

## NOTES

## RELATED LINKS
