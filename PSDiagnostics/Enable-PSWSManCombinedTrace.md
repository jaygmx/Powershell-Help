---
external help file: PSDiagnostics-help.xml
Module Name: PSDiagnostics
online version: https://docs.microsoft.com/powershell/module/psdiagnostics/enable-pswsmancombinedtrace?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Enable-PSWSManCombinedTrace

## SYNOPSIS
Start a logging session with the WSMan and PowerShell providers enabled.

## SYNTAX

```
Enable-PSWSManCombinedTrace [-DoNotOverwriteExistingTrace]
```

## DESCRIPTION
\> This cmdlet is only available on the Windows platform.
This cmdlet starts a logging session with the following PowerShell providers enabled:

- Microsoft-Windows-PowerShell
- Microsoft-Windows-WinRM

The session is named 'PSTrace'.

This cmdlet uses the \`Start-Trace\` cmdlet.

You must run this cmdlet from an elevated PowerShell session.

## EXAMPLES

### Example 1: Start a combined logging session
```
Enable-PSWSManCombinedTrace
```

## PARAMETERS

### -DoNotOverwriteExistingTrace
By default, the events are written to "$pshome\Traces\PSTrace.etl".
When this parameter is used, the cmdlet creates a unique filename: "$pshome\Traces\PSTrace_{guid}.etl"

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

## RELATED LINKS

[Event Tracing]()

[Start-Trace]()

[Disable-PSWSManCombinedTrace]()

