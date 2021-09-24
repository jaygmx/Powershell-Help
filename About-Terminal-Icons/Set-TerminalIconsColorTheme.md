---
external help file: Terminal-Icons-help.xml
Module Name:
online version:
schema: 2.0.0
---

# Set-TerminalIconsColorTheme

## SYNOPSIS
Set the Terminal-Icons color theme.

## SYNTAX

```
Set-TerminalIconsColorTheme [-Name] <String> [<CommonParameters>]
```

## DESCRIPTION
Set the Terminal-Icons color theme to a registered theme.

## EXAMPLES

### EXAMPLE 1
```
Set-TerminalIconsColorTheme -Name devblackops
```

Set the color theme to 'devblackops'.

## PARAMETERS

### -Name
The name of a registered color theme.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
### The name of a registered color theme.
## OUTPUTS

### None.
## NOTES
*

## RELATED LINKS

[Set-TerminalIconsIconTheme]()

[Get-TerminalIconsColorTheme]()

[Get-TerminalIconsIconTheme]()

