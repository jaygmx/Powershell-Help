---
external help file: PSDiagnostics-help.xml
Module Name: PSDiagnostics
online version: https://docs.microsoft.com/powershell/module/psdiagnostics/enable-pstrace?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Enable-PSTrace

## SYNOPSIS
Enables the Microsoft-Windows-PowerShell event provider logs.

## SYNTAX

```
Enable-PSTrace [-Force] [-AnalyticOnly]
```

## DESCRIPTION
\> This cmdlet is only available on the Windows platform.
This cmdlet enables the Operational and Analytic event logs of the Microsoft-Windows-PowerShell event provider.

You must run this cmdlet from an elevated PowerShell session.

## EXAMPLES

### Example 1: Enable the Analytic event log for PowerShell
```
Enable-PSTrace -AnalyticOnly
```

## PARAMETERS

### -AnalyticOnly
When this parameter is used, the cmdlet enables the Analytic event log of the Microsoft-Windows-PowerShell provider.
The Operational event log is not changed.

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
Used to force the change without prompting.

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

## INPUTS

### None
## OUTPUTS

### None
## NOTES
This cmdlet uses the \`Get-LogProperties\` and \`Set-LogProperties\` cmdlets.

You must run this cmdlet from an elevated PowerShell session.

## RELATED LINKS

[Get-LogProperties]()

[Set-LogProperties]()

[Disable-PSTrace]()

