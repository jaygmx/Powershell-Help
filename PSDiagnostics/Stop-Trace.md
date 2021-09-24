---
external help file: PSDiagnostics-help.xml
Module Name: PSDiagnostics
online version: https://docs.microsoft.com/powershell/module/psdiagnostics/stop-trace?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Stop-Trace

## SYNOPSIS
Stop an Event Trace logging session.

## SYNTAX

```
Stop-Trace [-SessionName] <Object> [-ETS] [<CommonParameters>]
```

## DESCRIPTION
\> This cmdlet is only available on the Windows platform.
This cmdlet stops a Windows Event Trace logging session.

This cmdlet is used by the following cmdlets:

- \`Disable-PSWSManCombinedTrace\`
- \`Disable-WSManTrace\`

You must run this cmdlet from an elevated PowerShell session.

## EXAMPLES

### Example 1: Stop a WSMan Trace logging session
```
Stop-Trace -SessionName 'wsmlog'
```

## PARAMETERS

### -ETS
Send commands to Event Trace Sessions directly without saving or scheduling.

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

### -SessionName
The name of the Event Trace session to be stopped.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### None
## NOTES

## RELATED LINKS

[Event Tracing]()

[Start-Trace]()

[Disable-PSWSManCombinedTrace]()

[Disable-WSManTrace]()

[Enable-PSWSManCombinedTrace]()

[Enable-WSManTrace]()

