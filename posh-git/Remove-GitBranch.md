---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Remove-GitBranch

## SYNOPSIS
Deletes the specified Git branches.

## SYNTAX

### Wildcard (Default)
```
Remove-GitBranch [-Name] <String> [-ExcludePattern <String>] [-Commit <String>] [-IncludeUnmerged] [-Force]
 [-DeleteForce] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Pattern
```
Remove-GitBranch [-Pattern] <String> [-ExcludePattern <String>] [-Commit <String>] [-IncludeUnmerged] [-Force]
 [-DeleteForce] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Deletes the specified Git branches that have been merged into the commit specified by the Commit parameter (HEAD by default).
You must either specify a branch name via the Name parameter, which accepts wildard characters, or via the Pattern parameter, which accepts a regular expression.

The following branches are always excluded from deletion:

* The current branch
* develop
* master

The default set of excluded branches can be overridden with the ExcludePattern parameter.

Consider always running this command FIRST with the WhatIf parameter.
This will show you which branches will be deleted.
This gives you a chance to adjust your branch name wildcard pattern or regular expression if you are using the Pattern parameter.

IMPORTANT: Be careful using this command.
Even though by default this command deletes only merged branches, most, if not all, of your historical branches have been merged.
But that doesn't mean you want to delete them.
That is why this command excludes \`develop\` and \`master\` by default.
But you may use different names e.g.
\`development\` or have other historical branches you don't want to delete.
In these cases, you can either:

* Specify a narrower branch name wildcard such as "user/$env:USERNAME/*".
* Specify an updated ExcludeParameter e.g.
'(^\*)|(^.
(develop|master|v\d+)$)' which adds any branch matching the pattern 'v\d+' to the exclusion list.

If necessary, you can delete the specified branches REGARDLESS of their merge status by using the IncludeUnmerged parameter.
BE VERY CAREFUL using the IncludeUnmerged parameter together with the Force parameter, since you will not be given the opportunity to confirm each branch deletion.

The following Git commands are executed by this command:

    git branch --merged $Commit |
        Where-Object { $_ -notmatch $ExcludePattern } |
        Where-Object { $_.Trim() -like $Name } |
        Foreach-Object { git branch --delete $_.Trim() }

If the IncludeUnmerged parameter is specified, execution changes to:

    git branch |
        Where-Object { $_ -notmatch $ExcludePattern } |
        Where-Object { $_.Trim() -like $Name } |
        Foreach-Object { git branch --delete $_.Trim() }

If the DeleteForce parameter is specified, the Foreach-Object changes to:

    Foreach-Object { git branch --delete --force $_.Trim() }

If the Pattern parameter is used instead of the Name parameter, the second Where-Object changes to:

    Where-Object { $_ -match $Pattern }

Recovering Deleted Branches

If you wind up deleting a branch you didn't intend to, you can easily recover it with the info provided by Git during the delete.
For instance, let's say you realized you didn't want to delete the branch 'feature/exp1'.
In the output of this command, you should see a deletion entry for this branch that looks like:

    Deleted branch feature/exp1 (was 08f9000).

To recover this branch, execute the following Git command:

    # git branch \<branch-name\> \<sha1\>
    git branch feature/exp1 08f9000

## EXAMPLES

### EXAMPLE 1
```
Remove-GitBranch -Name "user/${env:USERNAME}/*" -WhatIf
Shows the merged branches that would be deleted by the specified branch name without actually deleting. Remove the WhatIf parameter when you are happy with the list of branches that will be deleted.
```

### EXAMPLE 2
```
Remove-GitBranch "feature/*" -Force
Deletes the merged branches that match the specified wildcard. Using the Force parameter skips all confirmation prompts. Name is a positional parameter. The first argument is assumed to be the value of the Name parameter.
```

### EXAMPLE 3
```
Remove-GitBranch "bugfix/*" -Force -DeleteForce
Deletes the merged branches that match the specified wildcard. Using the Force parameter skips all confirmation prompts while the DeleteForce parameter uses the --force option in the underlying Git command.
```

### EXAMPLE 4
```
Remove-GitBranch -Pattern 'user/(dahlbyk|hillr)/.*'
Deletes the merged branches that match the specified regular expression.
```

### EXAMPLE 5
```
Remove-GitBranch -Name * -ExcludePattern '(^\*)|(^. (develop|master|v\d+)$)'
Deletes merged branches except the current branch, develop, master and branches that also match the pattern 'v\d+' e.g. v1, v1.0, v1.x. BE VERY CAREFUL SPECIYING SUCH A BROAD BRANCH NAME WILDCARD!
```

### EXAMPLE 6
```
Remove-GitBranch "feature/*" -IncludeUnmerged -WhatIf
Shows the branches, both merged and unmerged, that match the specified wildcard that would be deleted without actually deleting them. Once you've verified the list of branches looks correct, remove the WhatIf parameter to actually delete the branches.
```

## PARAMETERS

### -Name
Specifies a regular expression pattern for the branches that will be deleted.
Certain branches are always excluded from deletion e.g.
the current branch as well as the develop and master branches.
See the ExcludePattern parameter to modify that pattern.

```yaml
Type: System.String
Parameter Sets: Wildcard
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Pattern
Specifies a regular expression for the branches that will be deleted.
Certain branches are always excluded from deletion e.g.
the current branch as well as the develop and master branches.
See the ExcludePattern parameter to modify that pattern.

```yaml
Type: System.String
Parameter Sets: Pattern
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExcludePattern
Specifies a regular expression used to exclude merged branches from being deleted.
The default pattern excludes the current branch, develop and master branches.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: (^\*)|(^. (develop|master)$)
Accept pipeline input: False
Accept wildcard characters: False
```

### -Commit
Branches whose tips are reachable from the specified commit will be deleted.
The default commit is HEAD.
This parameter is ignored if the IncludeUnmerged parameter is specified.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: HEAD
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeUnmerged
Specifies that unmerged branches are also eligible to be deleted.

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
Deletes the specified branches without prompting for confirmation.
By default, Remove-GitBranch prompts for confirmation before deleting branches.

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

### -DeleteForce
Deletes the specified branches by adding the --force parameter to the git branch --delete command e.g.
git branch --delete --force \<branch-name\>.
This is also the equivalent of using the -D parameter on the git branch command.

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
