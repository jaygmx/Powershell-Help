---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Set-GcsObject

## SYNOPSIS


## SYNTAX

### FromBucketAndObjName
```
Set-GcsObject [[-Bucket] <String>] [-ObjectName] <String> [-PredefinedAcl <PredefinedAclEnum>]
 [<CommonParameters>]
```

### FromObjectObject
```
Set-GcsObject [-InputObject] <Object> [-PredefinedAcl <PredefinedAclEnum>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Bucket


```yaml
Type: System.String
Parameter Sets: FromBucketAndObjName
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject


```yaml
Type: Google.Apis.Storage.v1.Data.Object
Parameter Sets: FromObjectObject
Aliases: Object

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ObjectName


```yaml
Type: System.String
Parameter Sets: FromBucketAndObjName
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PredefinedAcl


```yaml
Type: System.Nullable`1[Google.Apis.Storage.v1.ObjectsResource+UpdateRequest+PredefinedAclEnum]
Parameter Sets: (All)
Aliases:
Accepted values: AuthenticatedRead, BucketOwnerFullControl, BucketOwnerRead, Private__, ProjectPrivate, PublicRead

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Storage.v1.Data.Object

## OUTPUTS

### Google.Apis.Storage.v1.Data.Object

## NOTES

## RELATED LINKS
