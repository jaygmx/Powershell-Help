---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one
schema: 2.0.0
---

# Stop-PSOneClipboardListener

## SYNOPSIS
Stops the clipboard monitor and ends the background thread.

## SYNTAX

```
Stop-PSOneClipboardListener
```

## DESCRIPTION
As long as the clipboard monitor is running in the background, any valid PowerShell code that is copied to the clipboard opens a new editor pane.
So it is important to stop the clipboard monitor when it is not useful anymore. 
Make sure you stop the clipboard monitor before you close the ISE.
If the background thread continues to run, the ISE window may close but the ISE process may still run.

## EXAMPLES

### EXAMPLE 1
```
Stop-PSOneClipboardListener
Stops the clipboard monitor, and ends the background thread.
```

## PARAMETERS

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
