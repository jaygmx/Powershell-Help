---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# New-BqTable

## SYNOPSIS
{{ Fill in the Synopsis }}

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
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Dataset
{{ Fill Dataset Description }}

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
{{ Fill DatasetId Description }}

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
{{ Fill Description Description }}

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
{{ Fill Expiration Description }}

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
{{ Fill InputObject Description }}

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
{{ Fill Name Description }}

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
{{ Fill Project Description }}

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
{{ Fill Schema Description }}

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
{{ Fill TableId Description }}

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
