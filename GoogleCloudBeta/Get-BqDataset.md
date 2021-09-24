---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Get-BqDataset

## SYNOPSIS


## SYNTAX

### List
```
Get-BqDataset [-Project <String>] [-IncludeHidden] [-Filter <String[]>] [<CommonParameters>]
```

### GetWithString
```
Get-BqDataset [-Project <String>] [-DatasetId] <String> [<CommonParameters>]
```

### GetWithRef
```
Get-BqDataset [-Project <String>] [-Dataset] <DatasetReference> [<CommonParameters>]
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
Parameter Sets: GetWithRef
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DatasetId


```yaml
Type: System.String
Parameter Sets: GetWithString
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Filter


```yaml
Type: System.String[]
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeHidden


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: List
Aliases: All

Required: False
Position: Named
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

### Google.Apis.Bigquery.v2.Data.DatasetReference

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
