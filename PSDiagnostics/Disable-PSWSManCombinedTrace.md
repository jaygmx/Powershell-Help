---
external help file: PSDiagnostics-help.xml
Module Name: PSDiagnostics
online version: https://docs.microsoft.com/powershell/module/psdiagnostics/disable-pswsmancombinedtrace?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Disable-PSWSManCombinedTrace

## SYNOPSIS
Stop the logging session started by Enable-PSWSManCombinedTrace.

## SYNTAX

```
Disable-PSWSManCombinedTrace
```

## DESCRIPTION
\> This cmdlet is only available on the Windows platform.
This cmdlet stops the logging session started by \`Enable-PSWSManCombinedTrace\`.

This cmdlet uses the \`Stop-Trace\` cmdlet.

You must run this cmdlet from an elevated PowerShell session.

## EXAMPLES

### Example 1: Disable the combined logging session
```
Disable-PSWSManCombinedTrace
```

## PARAMETERS

## INPUTS

### None
## OUTPUTS

### None
## NOTES

## RELATED LINKS

[Event Tracing]()

[Stop-Trace]()

[Enable-PSWSManCombinedTrace]()

