---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Write-GitStatus

## SYNOPSIS
Writes the Git status for repo. 
Typically, you use Write-VcsStatus
function instead of this one.

## SYNTAX

```
Write-GitStatus [[-Status] <Object>] [<CommonParameters>]
```

## DESCRIPTION
Writes the Git status for repo.
This includes the branch name, branch
status with respect to its remote (if exists), index status, working
dir status, working dir local status and stash count (optional).
Various settings from GitPromptSettngs are used to format and color
the Git status.

On systems that support ANSI terminal sequences, this method will
return a string containing ANSI sequences to color various parts of
the Git status string. 
This string can be written to the host and
the ANSI sequences will be interpreted and converted to the specified
behaviors which is typically setting the foreground and/or background
color of text.

## EXAMPLES

### EXAMPLE 1
```
Write-GitStatus (Get-GitStatus)
```

Writes the Git status for the current repo.

## PARAMETERS

### -Status
The Git status object that provides the status information to be written.
This object is retrieved via the Get-GitStatus command.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Management.Automation.PSCustomObject
###     This is PSCustomObject returned by Get-GitStatus
## OUTPUTS

### System.String
###     This command returns a System.String object.
## NOTES

## RELATED LINKS
