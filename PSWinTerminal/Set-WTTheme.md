---
external help file: PSWinTerminal-help.xml
Module Name: PSWinTerminal
online version: https://github.com/sassdawe/PSWinTerminal
schema: 2.0.0
---

# Set-WTTheme

## SYNOPSIS
Set-WTTheme will change current Windows Terminal theme

## SYNTAX

```
Set-WTTheme [-Theme] <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Set-WTTheme will change the current Windows Terminal theme.

## EXAMPLES

### EXAMPLE 1
```
Set-WTTheme "Campbell Powershell"
```

Set-WTTheme will set current Windows Terminal theme to 'Campbell Powershell'

## PARAMETERS

### -Theme
Name of theme
\[ArgumentCompleter(
               {
                   param($Command, $Parameter, $WordToComplete, $CommandAst, $FakeBoundParams)

                   if ($FakeBoundParams.Theme) {
                       ( Initialize-WTThemeList | where-object { $_ -like $FakeBoundParams.Theme } ) | foreach-object { "\`'$_\`'" }
                   } else {
                       Initialize-WTThemeList | foreach-object { "\`'$_\`'" }
                   }
               }
           )\]

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
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

### Name of the theme we want to use for the current Windows Terminal profile
## OUTPUTS

### None.
## NOTES

## RELATED LINKS

[https://github.com/sassdawe/PSWinTerminal](https://github.com/sassdawe/PSWinTerminal)

