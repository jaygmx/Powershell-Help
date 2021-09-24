---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Get-GitBranchStatusColor

## SYNOPSIS
Gets the colors to use for the branch status.

## SYNTAX

```
Get-GitBranchStatusColor [[-Status] <Object>] [<CommonParameters>]
```

## DESCRIPTION
Gets the colors to use for the branch status.
This color is typically
used for the branch name as well. 
The default color is specified by
$GitPromptSettins.BranchColor. 
But depending on the Git status object
passed in, the colors could be changed to match that of one these
other $GitPromptSettings: BranchBehindAndAheadStatusSymbol,
BranchBehindStatusSymbol or BranchAheadStatusSymbol.

## EXAMPLES

### EXAMPLE 1
```
$branchStatusColor = Get-GitBranchStatusColor (Get-GitStatus)
```

Returns a PoshGitTextSpan with the foreground and background colors
for the branch status.

## PARAMETERS

### -Status
The Git status object that provides branch status information.
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

### PoshGitTextSpan
###     A PoshGitTextSpan with colors reflecting those to be used by
###     branch status symbols.
## NOTES

## RELATED LINKS
