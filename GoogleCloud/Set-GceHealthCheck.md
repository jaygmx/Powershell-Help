---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Set-GceHealthCheck

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByHttpObject
```
Set-GceHealthCheck [-HttpObject] <HttpHealthCheck> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByHttpsObject
```
Set-GceHealthCheck [-HttpsObject] <HttpsHealthCheck> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

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

### -HttpObject
{{ Fill HttpObject Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.HttpHealthCheck
Parameter Sets: ByHttpObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -HttpsObject
{{ Fill HttpsObject Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.HttpsHealthCheck
Parameter Sets: ByHttpsObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
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

### Google.Apis.Compute.v1.Data.HttpHealthCheck

### Google.Apis.Compute.v1.Data.HttpsHealthCheck

## OUTPUTS

### Google.Apis.Compute.v1.Data.HttpHealthCheck

### Google.Apis.Compute.v1.Data.HttpsHealthCheck

## NOTES

## RELATED LINKS
