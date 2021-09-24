---
external help file: PSDiagnostics-help.xml
Module Name: PSDiagnostics
online version: https://docs.microsoft.com/powershell/module/psdiagnostics/enable-wsmantrace?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Enable-WSManTrace

## SYNOPSIS
Start a logging session with the WSMan providers enabled.

## SYNTAX

```
Enable-WSManTrace
```

## DESCRIPTION
\> This cmdlet is only available on the Windows platform.
This cmdlet starts a logging session with the WSMan providers enabled.
The following event providers are enabled:

- Event Forwarding
- IpmiDrv
- IPMIPrv
- WinRM
- WinrsCmd
- WinrsExe
- WinrsMgr
- WSManProvHost

The session is named 'wsmlog'.

This cmdlet uses the \`Start-Trace\` cmdlet.

You must run this cmdlet from an elevated PowerShell session.

## EXAMPLES

### Example 1: Start a WSMan logging session.
```
Enable-WSManTrace
```

## PARAMETERS

## INPUTS

### None
## OUTPUTS

### None
## NOTES

## RELATED LINKS

[Event Tracing]()

[Start-Trace]()

[Disable-WSManTrace]()

