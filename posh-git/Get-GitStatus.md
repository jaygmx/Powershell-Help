---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Get-GitStatus

## SYNOPSIS
Gets a Git status object that is used by \`Write-GitStatus\`.

## SYNTAX

```
Get-GitStatus [[-GitDir] <Object>] [-Force] [<CommonParameters>]
```

## DESCRIPTION
The \`Get-GitStatus\` cmdlet gets the status of the current Git repo.

The status object returned by this cmdlet provides the information
displayed in the various sections of the posh-git prompt.
The following
properties in $GitPromptSettings control what information is returned in
the status object:

EnableFileStatus          = $true # Or $false if Git not installed
EnableFileStatusFromCache = \<unset\> # Or $true if GitStatusCachePoshClient installed
EnablePromptStatus        = $true
EnableStashStatus         = $false
UntrackedFilesMode        = Default # Other enum values: No, Normal, All

The \`Force\` parameter can be used to override the EnableFileStatus and
EnablePromptStatus properties to ensure that both file and prompt status
information is returned in the status object.

## EXAMPLES

### EXAMPLE 1
```
$s = Get-GitStatus; Write-GitStatus $s
Gets a Git status object. Then passes the object to Write-GitStatus which
writes out a posh-git prompt (or returns a string in ANSI mode) with the
information contained in the status object.
```

### EXAMPLE 2
```
$s = Get-GitStatus -Force
Gets a Git status object that always returns all status information even
if $GitPromptSettings has disabled `EnableFileStatus` and/or
`EnablePromptStatus`.
```

## PARAMETERS

### -GitDir
The path of a directory within a Git repository that you want to get
the Git status.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: (Get-GitDirectory)
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
If specified, overrides $GitPromptSettings.EnableFileStatus and
$GitPromptSettings.EnablePromptStatus when they are set to $false.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### System.Management.Automation.PSObject
## NOTES

## RELATED LINKS

[Write-GitStatus]()

