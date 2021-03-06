---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# New-BqTable

## SYNOPSIS


## SYNTAX

### ByObject
```
New-BqTable -InputObject <Table> [<CommonParameters>]
```

### ByValue
```
New-BqTable [-Project <String>] -DatasetId <String> [-TableId] <String> [-Name <String>]
 [-Description <String>] [-Expiration <Int64>] [-Schema <TableSchema>] [<CommonParameters>]
```

### ByValueWithRef
```
New-BqTable -Dataset <DatasetReference> [-TableId] <String> [-Name <String>] [-Description <String>]
 [-Expiration <Int64>] [-Schema <TableSchema>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Dataset


```yaml
Type: Google.Apis.Bigquery.v2.Data.DatasetReference
Parameter Sets: ByValueWithRef
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DatasetId


```yaml
Type: System.String
Parameter Sets: ByValue
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Description


```yaml
Type: System.String
Parameter Sets: ByValue, ByValueWithRef
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Expiration


```yaml
Type: System.Int64
Parameter Sets: ByValue, ByValueWithRef
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject


```yaml
Type: Google.Apis.Bigquery.v2.Data.Table
Parameter Sets: ByObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name


```yaml
Type: System.String
Parameter Sets: ByValue, ByValueWithRef
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
Parameter Sets: ByValue
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Schema


```yaml
Type: Google.Apis.Bigquery.v2.Data.TableSchema
Parameter Sets: ByValue, ByValueWithRef
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TableId


```yaml
Type: System.String
Parameter Sets: ByValue, ByValueWithRef
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Bigquery.v2.Data.Table

### System.String

### Google.Apis.Bigquery.v2.Data.DatasetReference

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
