---
external help file: posh-git-help.xml
Module Name: posh-git
online version:
schema: 2.0.0
---

# Write-Prompt

## SYNOPSIS
Writes the object to the display or renders it as a string using ANSI/VT sequences.

## SYNTAX

### Default (Default)
```
Write-Prompt [-Object] <Object> [-ForegroundColor <Object>] [-BackgroundColor <Object>]
 [-StringBuilder <StringBuilder>] [<CommonParameters>]
```

### CellColor
```
Write-Prompt [-Object] <Object> [-Color <PoshGitCellColor>] [-StringBuilder <StringBuilder>]
 [<CommonParameters>]
```

## DESCRIPTION
Writes the specified object to the display unless $GitPromptSettings.AnsiConsole
is enabled. 
In this case, the Object is rendered, along with the specified
colors, as a string with the appropriate ANSI/VT sequences for colors embedded
in the string. 
If a StringBuilder is provided, the string is appended to the
StringBuilder.

## EXAMPLES

### EXAMPLE 1
```
Write-Prompt "PS > " -ForegroundColor Cyan -BackgroundColor Black
On a system where $GitPromptSettings.AnsiConsole is set to $false, this
will write the above to the display using the Write-Host command.
If AnsiConsole is set to $true, this will return a string of the form:
"`e[96m`e[40mPS > `e[0m".
```

### EXAMPLE 2
```
$sb = [System.Text.StringBuilder]::new()
PS C:\> $sb | Write-Prompt "PS > " -ForegroundColor Cyan -BackgroundColor Black
On a system where $GitPromptSettings.AnsiConsole is set to $false, this
will write the above to the display using the Write-Host command.
If AnsiConsole is set to $true, this will append the following string to the
StringBuilder object piped into the command:
"`e[96m`e[40mPS > `e[0m".
```

## PARAMETERS

### -Object
Specifies objects to display in the console or render as a string if
$GitPromptSettings.AnsiConsole is enabled.
If the Object is of type
\[PoshGitTextSpan\] the other color parameters are ignored since a
\[PoshGitTextSpan\] provides the colors.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForegroundColor
Specifies the foreground color.

```yaml
Type: System.Object
Parameter Sets: Default
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
Specifies the background color.

```yaml
Type: System.Object
Parameter Sets: Default
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color
Specifies both the background and foreground colors via \[PoshGitCellColor\] object.

```yaml
Type: PoshGitCellColor
Parameter Sets: CellColor
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StringBuilder
When specified and $GitPromptSettings.AnsiConsole is enabled, the Object parameter
is written to the StringBuilder along with the appropriate ANSI/VT sequences for
the specified foreground and background colors.

```yaml
Type: System.Text.StringBuilder
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
