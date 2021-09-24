---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Write-GitWorkingDirStatusSummary

## SYNOPSIS
Writes the working directory status summary text given the current Git status.

## SYNTAX

```
Write-GitWorkingDirStatusSummary [[-Status] <Object>] [-StringBuilder <StringBuilder>] [-NoLeadingSpace]
 [<CommonParameters>]
```

## DESCRIPTION
Writes the working directory status summary text given the current Git status.
If there are any unstaged commits, the $GitPromptSettings.LocalWorkingStatusSymbol
will be output. 
If not, then if are any staged but uncommmited changes, the
$GitPromptSettings.LocalStagedStatusSymbol will be output. 
If not, then
$GitPromptSettings.LocalDefaultStatusSymbol will be output.

## EXAMPLES

### EXAMPLE 1
```
Write-GitWorkingDirStatusSummary (Get-GitStatus)
```

Outputs the Git working directory status summary text.

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

### -NoLeadingSpace
If specified, suppresses the output of the leading space character.

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

### System.Management.Automation.PSCustomObject
###     This is PSCustomObject returned by Get-GitStatus
## OUTPUTS

### System.String, System.Text.StringBuilder
###     This command returns a System.String object unless the -StringBuilder parameter
###     is supplied. In this case, it returns a System.Text.StringBuilder.
## NOTES

## RELATED LINKS
