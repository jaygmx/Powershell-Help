---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Get-BqTable

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByValue
```
Get-BqTable [-Project <String>] [[-Table] <String>] -DatasetId <String> [<CommonParameters>]
```

### ByDatasetObject
```
Get-BqTable [[-Table] <String>] -Dataset <DatasetReference> [<CommonParameters>]
```

### ByObject
```
Get-BqTable [-InputObject] <TableReference> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Dataset
{{ Fill Dataset Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.DatasetReference
Parameter Sets: ByDatasetObject
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
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
{{ Fill InputObject Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.TableReference
Parameter Sets: ByObject
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
Parameter Sets: ByValue
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Table
{{ Fill Table Description }}

```yaml
Type: System.String
Parameter Sets: ByValue, ByDatasetObject
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Bigquery.v2.Data.DatasetReference

### Google.Apis.Bigquery.v2.Data.TableReference

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
