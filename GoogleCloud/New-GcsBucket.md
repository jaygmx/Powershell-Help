---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcsBucket

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
New-GcsBucket [-Name] <String> [-Project <String>] [-StorageClass <String>] [-Location <String>]
 [-DefaultBucketAcl <PredefinedAclEnum>] [-DefaultObjectAcl <PredefinedDefaultObjectAclEnum>]
 [<CommonParameters>]
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

### -DefaultBucketAcl
{{ Fill DefaultBucketAcl Description }}

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
{{ Fill DefaultObjectAcl Description }}

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
{{ Fill Location Description }}

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
{{ Fill Name Description }}

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

### -StorageClass
{{ Fill StorageClass Description }}

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
