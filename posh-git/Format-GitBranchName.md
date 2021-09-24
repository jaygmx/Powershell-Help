---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Format-GitBranchName

## SYNOPSIS
Formats the branch name text according to $GitPromptSettings.

## SYNTAX

```
Format-GitBranchName [[-BranchName] <String>] [<CommonParameters>]
```

## DESCRIPTION
Formats the branch name text according the $GitPromptSettings:
BranchNameLimit and TruncatedBranchSuffix.

## EXAMPLES

### EXAMPLE 1
```
$branchName = Format-GitBranchName (Get-GitStatus).Branch
```

Gets the branch name formatted as specified by the user's $GitPromptSettings.

## PARAMETERS

### -BranchName
The branch name to format according to the GitPromptSettings:
BranchNameLimit and TruncatedBranchSuffix.

```yaml
Type: System.String
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

### System.String
###     This is the branch name as a string.
## OUTPUTS

### System.String
###     This command returns a System.String object.
## NOTES

## RELATED LINKS
