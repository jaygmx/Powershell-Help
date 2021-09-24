---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Add-PoshGitToProfile

## SYNOPSIS
Configures your PowerShell profile (startup) script to import the posh-git
module when PowerShell starts.

## SYNTAX

```
Add-PoshGitToProfile [-AllHosts] [-AllUsers] [-Force] [[-TestParams] <PSObject[]>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Checks if your PowerShell profile script is not already importing posh-git
and if not, adds a command to import the posh-git module.
This will cause
PowerShell to load posh-git whenever PowerShell starts.

## EXAMPLES

### EXAMPLE 1
```
Add-PoshGitToProfile
Updates your profile script for the current PowerShell host to import the
posh-git module when the current PowerShell host starts.
```

### EXAMPLE 2
```
Add-PoshGitToProfile -AllHosts
Updates your profile script for all PowerShell hosts to import the posh-git
module whenever any PowerShell host starts.
```

## PARAMETERS

### -AllHosts
By default, this command modifies the CurrentUserCurrentHost profile
script. 
By specifying the AllHosts switch, the command updates the
CurrentUserAllHosts profile (or AllUsersAllHosts, given -AllUsers).

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllUsers
By default, this command modifies the CurrentUserCurrentHost profile
script. 
By specifying the AllUsers switch, the command updates the
AllUsersCurrentHost profile (or AllUsersAllHosts, given -AllHosts).
Requires elevated permissions.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Do not check if the specified profile script is already importing
posh-git.
Just add Import-Module posh-git command.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -TestParams
{{ Fill TestParams Description }}

```yaml
Type: System.Management.Automation.PSObject[]
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

### None.
## OUTPUTS

### None.
## NOTES

## RELATED LINKS
