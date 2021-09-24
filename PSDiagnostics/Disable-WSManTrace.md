---
external help file: PSDiagnostics-help.xml
Module Name: PSDiagnostics
online version: https://docs.microsoft.com/powershell/module/psdiagnostics/disable-wsmantrace?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Disable-WSManTrace

## SYNOPSIS
Stop the WSMan logging session started by Enable-WSManTrace.

## SYNTAX

```
Disable-WSManTrace
```

## DESCRIPTION
\> This cmdlet is only available on the Windows platform.
This cmdlet stops the WSMan logging session started by Enable-WSManTrace.

This cmdlet uses the \`Stop-Trace\` cmdlet.

You must run this cmdlet from an elevated PowerShell session.

## EXAMPLES

### Example 1: Stop a WSMan trace
```
Disable-WSManTrace
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

[Enable-WSManTrace]()

