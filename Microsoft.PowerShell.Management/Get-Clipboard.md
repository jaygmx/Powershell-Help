---
external help file: Microsoft.PowerShell.Commands.Management.dll-Help.xml
Module Name: Microsoft.PowerShell.Management
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.management/get-clipboard?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Get-Clipboard

## SYNOPSIS
Gets the contents of the clipboard.

## SYNTAX

```
Get-Clipboard [-Raw] [<CommonParameters>]
```

## DESCRIPTION
\> This cmdlet is not supported on macOS.
The \`Get-Clipboard\` cmdlet gets the contents of the clipboard as text.
Multiple lines of text are returned as an array of strings similar to \`Get-Content\`.

\> \[!NOTE\] \> On Linux, this cmdlet requires the \`xclip\` utility to be in the path.

## EXAMPLES

### Example 1: Get the content of the clipboard and display it to the command-line
```
Get-Clipboard

hello
```

## PARAMETERS

### -Raw
Gets the entire contents of the clipboard.
Multiline text is returned as a single multiline string rather than an array of strings.

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

### System.String
## NOTES

## RELATED LINKS

[Set-Clipboard]()

