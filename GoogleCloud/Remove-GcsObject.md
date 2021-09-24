---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Remove-GcsObject

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### FromObjectName (Default)
```
Remove-GcsObject [[-Bucket] <String>] [-ObjectName] <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### FromObjectObject
```
Remove-GcsObject [-InputObject] <Object> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Bucket
{{ Fill Bucket Description }}

```yaml
Type: System.String
Parameter Sets: FromObjectName
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -InputObject
{{ Fill InputObject Description }}

```yaml
Type: Google.Apis.Storage.v1.Data.Object
Parameter Sets: FromObjectObject
Aliases: Object

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ObjectName
{{ Fill ObjectName Description }}

```yaml
Type: System.String
Parameter Sets: FromObjectName
Aliases:

Required: True
Position: 1
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

### Google.Apis.Storage.v1.Data.Object

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
