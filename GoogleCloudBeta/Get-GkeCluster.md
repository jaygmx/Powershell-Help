---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Get-GkeCluster

## SYNOPSIS


## SYNTAX

### AllZone (Default)
```
Get-GkeCluster [-Project <String>] [<CommonParameters>]
```

### ByZone
```
Get-GkeCluster [-Project <String>] -Zone <String> [<CommonParameters>]
```

### ByName
```
Get-GkeCluster [-Project <String>] [-Zone <String>] [-ClusterName] <String[]> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -ClusterName


```yaml
Type: System.String[]
Parameter Sets: ByName
Aliases: Name

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

### -Zone


```yaml
Type: System.String
Parameter Sets: ByZone
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

### None

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
