---
external help file: Microsoft.PowerShell.PSReadLine2.dll-help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-PSReadLineOption

## SYNOPSIS
Returns the values for the options that can be configured.

## SYNTAX

```
Get-PSReadLineOption [<CommonParameters>]
```

## DESCRIPTION
Get-PSReadLineOption returns the current state of the settings that can be configured by Set-PSReadLineOption.

The object returned can be used to change PSReadLine options.

This provides a slightly simpler way of setting syntax coloring options for multiple kinds of tokens.

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```



## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
You cannot pipe objects to Get-PSReadLineOption

## OUTPUTS

### Microsoft.PowerShell.PSConsoleReadLineOptions
An instance of the current options.
Changing the values will update the settings in PSReadLine directly without invoking Set-PSReadLineOption.

## NOTES
*

## RELATED LINKS

[about_PSReadLine]()

