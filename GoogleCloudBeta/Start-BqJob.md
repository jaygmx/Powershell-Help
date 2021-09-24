---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Start-BqJob

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### DoQuery
```
Start-BqJob [-Project <String>] [-PollUntilComplete] [-Query] [-QueryString] <String> [-UseLegacySql]
 [-DefaultDataset <DatasetReference>] [-Priority <QueryPriority>] [[-Destination] <TableReference>]
 [-WriteMode <WriteDisposition>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### DoCopy
```
Start-BqJob [-Project <String>] [-PollUntilComplete] [-Copy] -Source <TableReference>
 [-Destination] <TableReference> [-WriteMode <WriteDisposition>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### DoExtract
```
Start-BqJob [-Project <String>] [-PollUntilComplete] -Source <TableReference> [-Type] <DataFormats>
 [-FieldDelimiter <String>] [-Extract] [-DestinationUris] <String[]> [-Compress] [-NoHeader] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### DoLoad
```
Start-BqJob [-Project <String>] [-PollUntilComplete] [-Destination] <TableReference>
 [-WriteMode <WriteDisposition>] [-Load] [-Type] <DataFormats> [-SourceUris] <String[]> [-Encoding <String>]
 [-FieldDelimiter <String>] [-Quote <String>] [-SkipLeadingRows <Int32>] [-AllowUnknownFields]
 [-AllowJaggedRows] [-AllowQuotedNewlines] [-MaxBadRecords <Int32>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -AllowJaggedRows
{{ Fill AllowJaggedRows Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DoLoad
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
Parameter Sets: DoLoad
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
Parameter Sets: DoLoad
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Compress
{{ Fill Compress Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DoExtract
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Copy
{{ Fill Copy Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DoCopy
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultDataset
{{ Fill DefaultDataset Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.DatasetReference
Parameter Sets: DoQuery
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Destination
{{ Fill Destination Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.TableReference
Parameter Sets: DoQuery
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: Google.Apis.Bigquery.v2.Data.TableReference
Parameter Sets: DoCopy
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: Google.Apis.Bigquery.v2.Data.TableReference
Parameter Sets: DoLoad
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestinationUris
{{ Fill DestinationUris Description }}

```yaml
Type: System.String[]
Parameter Sets: DoExtract
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Encoding
{{ Fill Encoding Description }}

```yaml
Type: System.String
Parameter Sets: DoLoad
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Extract
{{ Fill Extract Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DoExtract
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FieldDelimiter
{{ Fill FieldDelimiter Description }}

```yaml
Type: System.String
Parameter Sets: DoExtract, DoLoad
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Load
{{ Fill Load Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DoLoad
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxBadRecords
{{ Fill MaxBadRecords Description }}

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: DoLoad
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoHeader
{{ Fill NoHeader Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DoExtract
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PollUntilComplete
{{ Fill PollUntilComplete Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: Synchronous

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Priority
{{ Fill Priority Description }}

```yaml
Type: Google.Cloud.BigQuery.V2.QueryPriority
Parameter Sets: DoQuery
Aliases:
Accepted values: Interactive, Batch

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
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Query
{{ Fill Query Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DoQuery
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -QueryString
{{ Fill QueryString Description }}

```yaml
Type: System.String
Parameter Sets: DoQuery
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Quote
{{ Fill Quote Description }}

```yaml
Type: System.String
Parameter Sets: DoLoad
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
Type: System.Nullable`1[System.Int32]
Parameter Sets: DoLoad
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Source
{{ Fill Source Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.TableReference
Parameter Sets: DoCopy, DoExtract
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SourceUris
{{ Fill SourceUris Description }}

```yaml
Type: System.String[]
Parameter Sets: DoLoad
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
{{ Fill Type Description }}

```yaml
Type: Google.PowerShell.BigQuery.DataFormats
Parameter Sets: DoExtract, DoLoad
Aliases:
Accepted values: AVRO, CSV, JSON, DATASTORE_BACKUP

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseLegacySql
{{ Fill UseLegacySql Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DoQuery
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WriteMode
{{ Fill WriteMode Description }}

```yaml
Type: System.Nullable`1[Google.Cloud.BigQuery.V2.WriteDisposition]
Parameter Sets: DoQuery, DoCopy, DoLoad
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
