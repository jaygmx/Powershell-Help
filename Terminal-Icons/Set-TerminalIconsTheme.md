---
external help file: Terminal-Icons-help.xml
Module Name: Terminal-Icons
online version:
schema: 2.0.0
---

# Set-TerminalIconsTheme

## SYNOPSIS
Set the Terminal-Icons color or icon theme

## SYNTAX

```
Set-TerminalIconsTheme [[-IconTheme] <String>] [[-ColorTheme] <String>] [-Force] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Set the Terminal-Icons color or icon theme to the given name.

## EXAMPLES

### EXAMPLE 1
```
Set-TerminalIconsTheme -ColorTheme devblackops
```

Set the color theme to 'devblackops'.

### EXAMPLE 2
```
Set-TerminalIconsTheme -IconTheme devblackops
```

Set the icon theme to 'devblackops'.

## PARAMETERS

### -IconTheme
The name of a registered icon theme to use.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColorTheme
The name of a registered color theme to use.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Bypass confirmation messages.

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

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
### The name of the color or icon theme to use.
## OUTPUTS

### None.
## NOTES
This function supercedes Set-TerminalIconsColorTheme and Set-TerminalIconsIconTheme.
They have been deprecated.

## RELATED LINKS

[Get-TerminalIconsColorTheme]()

[Get-TerminalIconsIconTheme]()

[Get-TerminalIconsTheme]()

