---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Get-BqJob

## SYNOPSIS


## SYNTAX

### List (Default)
```
Get-BqJob [-Project <String>] [-State <StateFilterEnum>] [-AllUsers] [<CommonParameters>]
```

### GetString
```
Get-BqJob [-Project <String>] [[-JobId] <String>] [<CommonParameters>]
```

### GetObject
```
Get-BqJob [-Project <String>] [[-InputObject] <JobReference>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -AllUsers


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject


```yaml
Type: Google.Apis.Bigquery.v2.Data.JobReference
Parameter Sets: GetObject
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -JobId


```yaml
Type: System.String
Parameter Sets: GetString
Aliases:

Required: False
Position: 0
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

### -State


```yaml
Type: Google.Apis.Bigquery.v2.JobsResource+ListRequest+StateFilterEnum
Parameter Sets: List
Aliases:
Accepted values: Done, Pending, Running

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Bigquery.v2.Data.JobReference

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
