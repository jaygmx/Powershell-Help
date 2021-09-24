---
external help file: PSDesiredStateConfiguration-help.xml
Module Name: PSDesiredStateConfiguration
online version: https://docs.microsoft.com/powershell/module/psdesiredstateconfiguration/get-dscresource?view=powershell-7&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Invoke-DscResource

## SYNOPSIS


## SYNTAX

```
Invoke-DscResource [-Name] <String> [[-ModuleName] <ModuleSpecification>] [-Method] <String>
 [-Property] <Hashtable> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Method


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: Get, Set, Test

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ModuleName


```yaml
Type: Microsoft.PowerShell.Commands.ModuleSpecification
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Name


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Property


```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

### Microsoft.PowerShell.Commands.ModuleSpecification

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
