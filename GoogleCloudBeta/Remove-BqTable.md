---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Remove-BqTable

## SYNOPSIS


## SYNTAX

### ByValue
```
Remove-BqTable [-Project <String>] [-TableId] <String> -DatasetId <String> [-Force] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ByDatasetObject
```
Remove-BqTable [-TableId] <String> -Dataset <DatasetReference> [-Force] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ByObject
```
Remove-BqTable [-Table] <TableReference> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

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

### -Dataset


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

### -Force


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

### -Table


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

### -TableId


```yaml
Type: System.String
Parameter Sets: ByValue, ByDatasetObject
Aliases:

Required: True
Position: 0
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Bigquery.v2.Data.DatasetReference

### Google.Apis.Bigquery.v2.Data.TableReference

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
