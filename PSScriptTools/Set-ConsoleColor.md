---
external help file: PSScriptTools-help.xml
Module Name: PSScriptTools
online version: http://bit.ly/31SMpPn
schema: 2.0.0
---

# Set-ConsoleColor

## SYNOPSIS
Set the PowerShell console color.

## SYNTAX

```
Set-ConsoleColor [[-Foreground] <ConsoleColor>] [[-Background] <ConsoleColor>] [-ClearScreen] [-Passthru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
You can use this command to modify the PowerShell console's foreground and/or background color.
If you are running the PSReadline module, that module has its own commands, like Set-PSReadLineOption, that you can use to modify your console.
Set-ConsoleColor is designed for use in a traditional PowerShell console.
It will not work in consoles that are part of the PowerShell ISE or Visual Studio Code.

## EXAMPLES

### Example 1
```
PS C:\> Set-ConsoleColor -foreground Yellow -background DarkGray -clear
```

Set the console color to yellow text and on a dark gray background.

## PARAMETERS

### -Background
Specify a background console color

```yaml
Type: System.ConsoleColor
Parameter Sets: (All)
Aliases: bg
Accepted values: Black, DarkBlue, DarkGreen, DarkCyan, DarkRed, DarkMagenta, DarkYellow, Gray, DarkGray, Blue, Green, Cyan, Red, Magenta, Yellow, White

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClearScreen
Clear the console host screen.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cls

Required: False
Position: Named
Default value: False
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
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Foreground
Specify a foreground console color.

```yaml
Type: System.ConsoleColor
Parameter Sets: (All)
Aliases: fg
Accepted values: Black, DarkBlue, DarkGreen, DarkCyan, DarkRed, DarkMagenta, DarkYellow, Gray, DarkGray, Blue, Green, Cyan, Red, Magenta, Yellow, White

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Passthru
Display the foreground and background color values.

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
Default value: False
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
Learn more about PowerShell: http://jdhitsolutions.com/blog/essential-powershell-resources/

## RELATED LINKS

[Set-ConsoleTitle]()

