---
external help file: AdminToolbox.ActiveDirectory-help.xml
Module Name: AdminToolbox.ActiveDirectory
online version:
schema: 2.0.0
---

# Get-DCLockoutEvents2

## SYNOPSIS

## SYNTAX

```
Get-DCLockoutEvents2 [-Identity] <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Parse Logs 4740 and 4776 on the PDCEmulator for workstations causing a lockout.
Null lockout location events are filtered.
Best if run shortly after a lockout.

## EXAMPLES

### EXAMPLE 1
```
Get-DCLockoutEvents2 -identity Joe
```

## PARAMETERS

### -Identity
Account that is being searched for lockout events

```yaml
Type: System.String
Parameter Sets: (All)
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
Requires The Active Directory Module

## RELATED LINKS

[Get-LockedAccounts
Get-PasswordExpired
Unlock-Account
Unlock-AllAccounts]()

