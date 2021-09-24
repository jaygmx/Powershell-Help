---
external help file: windows-screenfetch-help.xml
Module Name: windows-screenfetch
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/get-uptime?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Get-Uptime

## SYNOPSIS
Get the TimeSpan since last boot.

## SYNTAX

```
Get-Uptime
```

## DESCRIPTION
This cmdlet returns the time elapsed since the last boot of the operating system.

The \`Get-Uptime\` cmdlet was introduced in PowerShell 6.0.

## EXAMPLES

### Example 1 - Show time since last boot
```
Get-Uptime

Days              : 9
Hours             : 0
Minutes           : 9
Seconds           : 45
Milliseconds      : 0
Ticks             : 7781850000000
TotalDays         : 9.00677083333333
TotalHours        : 216.1625
TotalMinutes      : 12969.75
TotalSeconds      : 778185
TotalMilliseconds : 778185000
```

### Example 2 - Show the time of the last boot
```
Get-Uptime -Since

Tuesday, June 18, 2019 2:34:56 PM
```

## PARAMETERS

## INPUTS

### None

### None
## OUTPUTS

### System.Object
### System.TimeSpan
This is the default return type when no parameters are used.

### System.DateTime
This type is returned when using the Since parameter.

\> \[!NOTE\] \> If Windows fast startup is enabled, Windows does not update the value stored in \> LastBootUpTime .
To disable fast startup, run the following command: \`Powercfg -h off\`.
\> \> For more information about Windows fast startup, see \> Distinguishing Fast Startup from Wake-from-Hibernation (/windows-hardware/drivers/kernel/distinguishing-fast-startup-from-wake-from-hibernation).

## NOTES
On Windows, the value returned is the same as the LastBootUpTime property of the Win32_OperatingSystem class in WMI.

## RELATED LINKS

[Win32_OperatingSystem]()

