---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one
schema: 2.0.0
---

# Start-PSOneClipboardListener

## SYNOPSIS
Monitors the clipboard, and when new valid PowerShell code is detected, opens the code in an editor

## SYNTAX

```
Start-PSOneClipboardListener
```

## DESCRIPTION
Uses a background thread to monitor the clipboard.
If new valid PowerShell code is detected, an action is invoked.
The action depends on the editor used, and opens the clipboard code in an editor window

## EXAMPLES

### EXAMPLE 1
```
Start-PSOneClipboardListener
Starts the background clipboard monitor
```

## PARAMETERS

## INPUTS

## OUTPUTS

## NOTES
Anything that is copied to the clipboard can trigger the monitor, so make sure you turn off the monitor once you are done.

## RELATED LINKS

[https://powershell.one](https://powershell.one)

