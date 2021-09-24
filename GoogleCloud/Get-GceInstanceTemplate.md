---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Get-GceInstanceTemplate

## SYNOPSIS


## SYNTAX

### default (Default)
```
Get-GceInstanceTemplate [-Project <String>] [<CommonParameters>]
```

### byName
```
Get-GceInstanceTemplate [-Project <String>] [-Name] <String> [<CommonParameters>]
```

### byObject
```
Get-GceInstanceTemplate [-Object] <InstanceTemplate> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Name


```yaml
Type: System.String
Parameter Sets: byName
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Object


```yaml
Type: Google.Apis.Compute.v1.Data.InstanceTemplate
Parameter Sets: byObject
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
Parameter Sets: default, byName
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

### Google.Apis.Compute.v1.Data.InstanceTemplate

## OUTPUTS

### Google.Apis.Compute.v1.Data.InstanceTemplate

## NOTES

## RELATED LINKS
