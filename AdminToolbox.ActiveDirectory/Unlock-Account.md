---
external help file: AdminToolbox.ActiveDirectory-help.xml
Module Name: AdminToolbox.ActiveDirectory
online version:
schema: 2.0.0
---

# Unlock-Account

## SYNOPSIS

## SYNTAX

```
Unlock-Account [-Username] <Object> [<CommonParameters>]
```

## DESCRIPTION
Unlocks an Active Directory Account

## EXAMPLES

### EXAMPLE 1
```
Use Get-lockedAccounts to quickly obtain the identity to use in the command.
```

Get-LockedAccounts
Unlock-ADAccount -identity JohnD

## PARAMETERS

### -Username
Username of account being unlocked

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Requires the Active Directory Module.

## RELATED LINKS

[Get-DCLockoutEvents2
Get-LockedAccounts
Get-PasswordExpired
Set-Password
Unlock-AllAccounts]()

