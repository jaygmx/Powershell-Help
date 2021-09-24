---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Write-GitStashCount

## SYNOPSIS
Writes the stash count given the current Git status.

## SYNTAX

```
Write-GitStashCount [[-Status] <Object>] [-StringBuilder <StringBuilder>] [<CommonParameters>]
```

## DESCRIPTION
Writes the stash count given the current Git status.

## EXAMPLES

### EXAMPLE 1
```
Write-GitStashCount (Get-GitStatus)
```

Writes the Git stash count to the host.

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

### -StringBuilder
If specified the working dir local status is written into the provided StringBuilder object.

```yaml
Type: System.Text.StringBuilder
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Management.Automation.PSCustomObject
###     This is PSCustomObject returned by Get-GitStatus
## OUTPUTS

### System.String, System.Text.StringBuilder
###     This command returns a System.String object unless the -StringBuilder parameter
###     is supplied. In this case, it returns a System.Text.StringBuilder.
## NOTES

## RELATED LINKS
