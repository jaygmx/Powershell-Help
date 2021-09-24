---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Add-BqTableRow

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
Add-BqTableRow -InputObject <TableReference> [-Type] <DataFormats> [-Filename] <String>
 [-WriteMode <WriteDisposition>] [-AllowUnknownFields] [-AllowJaggedRows] [-AllowQuotedNewlines]
 [-FieldDelimiter <String>] [-Quote <String>] [-SkipLeadingRows <Int32>] [<CommonParameters>]
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

### -AllowJaggedRows
{{ Fill AllowJaggedRows Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowQuotedNewlines
{{ Fill AllowQuotedNewlines Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowUnknownFields
{{ Fill AllowUnknownFields Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FieldDelimiter
{{ Fill FieldDelimiter Description }}

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

### -Filename
{{ Fill Filename Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
{{ Fill InputObject Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.TableReference
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Quote
{{ Fill Quote Description }}

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

### -SkipLeadingRows
{{ Fill SkipLeadingRows Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
{{ Fill Type Description }}

```yaml
Type: Google.PowerShell.BigQuery.DataFormats
Parameter Sets: (All)
Aliases:
Accepted values: AVRO, CSV, JSON, DATASTORE_BACKUP

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WriteMode
{{ Fill WriteMode Description }}

```yaml
Type: Google.Cloud.BigQuery.V2.WriteDisposition
Parameter Sets: (All)
Aliases:
Accepted values: WriteAppend, WriteTruncate, WriteIfEmpty

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Bigquery.v2.Data.TableReference

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
