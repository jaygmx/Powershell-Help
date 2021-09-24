---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Set-ForegroundWindow

## SYNOPSIS
PSCX Cmdlet: Given an hWnd or window handle, brings that window to the foreground.
Useful for restoring a window to uppermost after an application which seizes the foreground is invoked.
See also Get-ForegroundWindow

## SYNTAX

```
Set-ForegroundWindow [[-Handle] <IntPtr>] [<CommonParameters>]
```

## DESCRIPTION
Given an hWnd or window handle, brings that window to the foreground.
Useful for restoring a window to uppermost after an application which seizes the foreground is invoked.
See also Get-ForegroundWindow

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Handle
handle for the window to be set as the foreground window.
If not specified, this defaults to the main window of the current process.

```yaml
Type: IntPtr
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS

[Get-ForegroundWindow]()

