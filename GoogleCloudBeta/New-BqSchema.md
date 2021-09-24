---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# New-BqSchema

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByValue
```
New-BqSchema [-PassThruObject <TableFieldSchema>] [-Name] <String> [-Type] <ColumnType>
 [[-Description] <String>] [[-Mode] <ColumnMode>] [-Fields <TableFieldSchema[]>] [<CommonParameters>]
```

### ByString
```
New-BqSchema [-PassThruObject <TableFieldSchema>] -JSON <String> [<CommonParameters>]
```

### ByFile
```
New-BqSchema [-PassThruObject <TableFieldSchema>] -Filename <String> [<CommonParameters>]
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
Parameter Sets: ByValue
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Fields
{{ Fill Fields Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.TableFieldSchema[]
Parameter Sets: ByValue
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filename
{{ Fill Filename Description }}

```yaml
Type: System.String
Parameter Sets: ByFile
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JSON
{{ Fill JSON Description }}

```yaml
Type: System.String
Parameter Sets: ByString
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Mode
{{ Fill Mode Description }}

```yaml
Type: System.Nullable`1[Google.PowerShell.BigQuery.ColumnMode]
Parameter Sets: ByValue
Aliases:
Accepted values: NULLABLE, REQUIRED, REPEATED

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
{{ Fill Name Description }}

```yaml
Type: System.String
Parameter Sets: ByValue
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThruObject
{{ Fill PassThruObject Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.TableFieldSchema
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Type
{{ Fill Type Description }}

```yaml
Type: Google.PowerShell.BigQuery.ColumnType
Parameter Sets: ByValue
Aliases:
Accepted values: STRING, BYTES, INTEGER, INT64, FLOAT, FLOAT64, BOOLEAN, BOOL, TIMESTAMP, DATE, TIME, DATETIME, RECORD, STRUCT

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Bigquery.v2.Data.TableFieldSchema

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
