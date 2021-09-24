---
external help file: AdminToolbox.FileManagement-help.xml
Module Name: AdminToolbox.FileManagement
online version:
schema: 2.0.0
---

# Remove-All

## SYNOPSIS

## SYNTAX

```
Remove-All [[-computer] <Object>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
This Command removes log files, temp files, and empties the recycle bin.
Access denied errors do not indicate a failure of the script.
Run for the local or a remote PC.

## EXAMPLES

### EXAMPLE 1
```
Free up space on the local computer
```

Remove-All

### EXAMPLE 2
```
Free up space on a remote PC. May be more effective if run locally depending on in place security.
```

Remove-All -Computer JackPC10

## PARAMETERS

### -computer
Specify a remote computer run cleanup against

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Remove-DisabledADProfiles
Remove-OlderThan]()

