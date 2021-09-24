---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcsBucket

## SYNOPSIS


## SYNTAX

```
New-GcsBucket [-Name] <String> [-Project <String>] [-StorageClass <String>] [-Location <String>]
 [-DefaultBucketAcl <PredefinedAclEnum>] [-DefaultObjectAcl <PredefinedDefaultObjectAclEnum>]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -DefaultBucketAcl


```yaml
Type: System.Nullable`1[Google.Apis.Storage.v1.BucketsResource+InsertRequest+PredefinedAclEnum]
Parameter Sets: (All)
Aliases:
Accepted values: AuthenticatedRead, Private__, ProjectPrivate, PublicRead, PublicReadWrite

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultObjectAcl


```yaml
Type: System.Nullable`1[Google.Apis.Storage.v1.BucketsResource+InsertRequest+PredefinedDefaultObjectAclEnum]
Parameter Sets: (All)
Aliases:
Accepted values: AuthenticatedRead, BucketOwnerFullControl, BucketOwnerRead, Private__, ProjectPrivate, PublicRead

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Location


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: ASIA, EU, US

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

Required: True
Position: 0
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

### -StorageClass


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: COLDLINE, DURABLE_REDUCED_AVAILABILITY, MULTI_REGIONAL, NEARLINE, REGIONAL, STANDARD

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Google.Apis.Storage.v1.Data.Bucket

## NOTES

## RELATED LINKS
