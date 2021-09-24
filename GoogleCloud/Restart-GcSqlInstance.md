---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Restart-GcSqlInstance

## SYNOPSIS


## SYNTAX

### ByName
```
Restart-GcSqlInstance [-Project <String>] [-Instance] <String> [<CommonParameters>]
```

### ByInstance
```
Restart-GcSqlInstance [-InstanceObject] <DatabaseInstance> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Instance


```yaml
Type: System.String
Parameter Sets: ByName
Aliases: Name, Id

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstanceObject


```yaml
Type: Google.Apis.SQLAdmin.v1beta4.Data.DatabaseInstance
Parameter Sets: ByInstance
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Project


```yaml
Type: System.String
Parameter Sets: ByName
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

### System.Object
## NOTES

## RELATED LINKS
