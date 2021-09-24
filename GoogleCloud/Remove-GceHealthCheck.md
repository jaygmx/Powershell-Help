---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Remove-GceHealthCheck

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByNameHttp
```
Remove-GceHealthCheck [-Project <String>] [-Name] <String> [-Http] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByNameHttps
```
Remove-GceHealthCheck [-Project <String>] [-Name] <String> [-Https] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByHttpObject
```
Remove-GceHealthCheck [-Http] [-HttpObject] <HttpHealthCheck> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByHttpsObject
```
Remove-GceHealthCheck [-Https] [-HttpsObject] <HttpsHealthCheck> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
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

### -Http
{{ Fill Http Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByNameHttp
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByHttpObject
Aliases:

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

### -Https
{{ Fill Https Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByNameHttps
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByHttpsObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### -Name
{{ Fill Name Description }}

```yaml
Type: System.String
Parameter Sets: ByNameHttp, ByNameHttps
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Project
{{ Fill Project Description }}

```yaml
Type: System.String
Parameter Sets: ByNameHttp, ByNameHttps
Aliases:

Required: False
Position: Named
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

### Google.Apis.Compute.v1.Data.HttpHealthCheck

### Google.Apis.Compute.v1.Data.HttpsHealthCheck

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
