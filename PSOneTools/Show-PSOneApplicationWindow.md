---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/powershell-internals/extending-powershell/vbscript-and-csharp
schema: 2.0.0
---

# Show-PSOneApplicationWindow

## SYNOPSIS
Brings main application window to the front (top most position on screen)

## SYNTAX

### Id (Default)
```
Show-PSOneApplicationWindow [-Id] <Int32> [-Maximize] [<CommonParameters>]
```

### Process
```
Show-PSOneApplicationWindow [-Process] <Process> [-Maximize] [<CommonParameters>]
```

## DESCRIPTION
Uses a number of strategies to force an application window to the top.

## EXAMPLES

### EXAMPLE 1
```
Show-PSOneApplicationWindow -Id $pid -Maximize 
Brings current PowerShell window to the top and maximizes the window
```

### EXAMPLE 2
```
Get-Process -Name Notepad | Show-PSOneApplicationWindow -Maximize
Brings notepad editor window to the top and maximizes it. 
If there is no notepad application running, an exception is thrown.
If there is more than one instance of notepad running, only the last instance is affected
```

## PARAMETERS

### -Id
Process Id of process. 
Process must have a main window and must not be hidden.

```yaml
Type: System.Int32
Parameter Sets: Id
Aliases:

Required: True
Position: 1
Default value: 0
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Process
Process.
Process must have a main window and must not be hidden.

```yaml
Type: System.Diagnostics.Process
Parameter Sets: Process
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Maximize
maximizes the window after it has been brought to the top

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

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one/powershell-internals/extending-powershell/vbscript-and-csharp](https://powershell.one/powershell-internals/extending-powershell/vbscript-and-csharp)

