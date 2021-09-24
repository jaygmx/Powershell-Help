---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Get-GceForwardingRule

## SYNOPSIS


## SYNTAX

### OfProject (Default)
```
Get-GceForwardingRule [-Project <String>] [-Global] [<CommonParameters>]
```

### ByGlobalName
```
Get-GceForwardingRule [-Project <String>] [-Global] [-Name] <String> [<CommonParameters>]
```

### OfRegion
```
Get-GceForwardingRule [-Project <String>] -Region <String> [<CommonParameters>]
```

### ByLocalName
```
Get-GceForwardingRule [-Project <String>] [-Region <String>] [-Name] <String> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Global


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: OfProject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByGlobalName
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name


```yaml
Type: System.String
Parameter Sets: ByGlobalName, ByLocalName
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

### -Region


```yaml
Type: System.String
Parameter Sets: OfRegion
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.String
Parameter Sets: ByLocalName
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

### Google.Apis.Compute.v1.Data.ForwardingRule

## NOTES

## RELATED LINKS
