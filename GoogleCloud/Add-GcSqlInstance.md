---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GcSqlInstance

## SYNOPSIS


## SYNTAX

### ByConfig
```
Add-GcSqlInstance [-Project <String>] [-InstanceConfig] <DatabaseInstance> [<CommonParameters>]
```

### Default
```
Add-GcSqlInstance [-Project <String>] [-Name] <String> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -InstanceConfig


```yaml
Type: Google.Apis.SQLAdmin.v1beta4.Data.DatabaseInstance
Parameter Sets: ByConfig
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name


```yaml
Type: System.String
Parameter Sets: Default
Aliases:

Required: True
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.SQLAdmin.v1beta4.Data.DatabaseInstance

## OUTPUTS

### Google.Apis.SQLAdmin.v1beta4.Data.DatabaseInstance

## NOTES

## RELATED LINKS
