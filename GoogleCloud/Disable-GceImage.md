---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Disable-GceImage

## SYNOPSIS


## SYNTAX

### ByName
```
Disable-GceImage [-Project <String>] [-Name] <String> [-Replacement <Image>] [-ReplacementUrl <String>]
 [-State] <ImageDisableState> [-DeprecateOn <DateTimeOffset>] [-ObsoleteOn <DateTimeOffset>]
 [-DeleteOn <DateTimeOffset>] [<CommonParameters>]
```

### ByObject
```
Disable-GceImage [-Object] <Image> [-Replacement <Image>] [-ReplacementUrl <String>]
 [-State] <ImageDisableState> [-DeprecateOn <DateTimeOffset>] [-ObsoleteOn <DateTimeOffset>]
 [-DeleteOn <DateTimeOffset>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -DeleteOn


```yaml
Type: System.Nullable`1[System.DateTimeOffset]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeprecateOn


```yaml
Type: System.Nullable`1[System.DateTimeOffset]
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
Type: Google.Apis.Compute.v1.Data.Image
Parameter Sets: ByObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ObsoleteOn


```yaml
Type: System.Nullable`1[System.DateTimeOffset]
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
Parameter Sets: ByName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Replacement


```yaml
Type: Google.Apis.Compute.v1.Data.Image
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplacementUrl


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

### -State


```yaml
Type: Google.PowerShell.ComputeEngine.DisableGceImageCmdlet+ImageDisableState
Parameter Sets: (All)
Aliases:
Accepted values: DEPRECATED, OBSOLETE, DELETED

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

### Google.Apis.Compute.v1.Data.Image

## OUTPUTS

### Google.Apis.Compute.v1.Data.Image

## NOTES

## RELATED LINKS
