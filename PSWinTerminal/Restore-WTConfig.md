---
external help file: PSWinTerminal-help.xml
Module Name: PSWinTerminal
online version: https://github.com/sassdawe/PSWinTerminal
schema: 2.0.0
---

# Restore-WTConfig

## SYNOPSIS
Restore-WTConfig will restore your Windows Terminal configuration.

## SYNTAX

```
Restore-WTConfig [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Restore-WTConfig will restore your Windows Terminal configuration to a backup which was created when the module was loaded into your current session.

The backup is stored in memory, and will be deleted when you close the current PowerShell session.

## EXAMPLES

### EXAMPLE 1
```
Restore-WTConfig
```

Restore-WTConfig will restore your Windows Terminal configuration

## PARAMETERS

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

### None.
## OUTPUTS

### None.
## NOTES

## RELATED LINKS

[https://github.com/sassdawe/PSWinTerminal](https://github.com/sassdawe/PSWinTerminal)

