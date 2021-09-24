---
external help file: PSWinTerminal-help.xml
Module Name: PSWinTerminal
online version:
schema: 2.0.0
---

# Import-WTTheme

## SYNOPSIS
Import-WTTheme

## SYNTAX

```
Import-WTTheme [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Import-WTTheme will import a valid scheme in JSON format from your clipboard

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

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

### [System.String] The content of your clipboard
## OUTPUTS

### [System.String] The name of the imported theme
## NOTES
You need to copy the scheme you want to import to your clipboard

## RELATED LINKS

[Sites to look for themes for Windows Terminal:
https://terminalsplash.com/
https://atomcorp.github.io/themes/]()

