---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Set-BqDataset

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### Default (Default)
```
Set-BqDataset [-Project <String>] [-Dataset] <Dataset> [<CommonParameters>]
```

### SetLabel
```
Set-BqDataset [-Project <String>] [-Dataset] <Dataset> -SetLabel <Hashtable> [<CommonParameters>]
```

### ClearLabel
```
Set-BqDataset [-Project <String>] [-Dataset] <Dataset> -ClearLabel <String[]> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -ClearLabel
{{ Fill ClearLabel Description }}

```yaml
Type: System.String[]
Parameter Sets: ClearLabel
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Dataset
{{ Fill Dataset Description }}

```yaml
Type: Google.Apis.Bigquery.v2.Data.Dataset
Parameter Sets: (All)
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
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SetLabel
{{ Fill SetLabel Description }}

```yaml
Type: System.Collections.Hashtable
Parameter Sets: SetLabel
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Bigquery.v2.Data.Dataset

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
