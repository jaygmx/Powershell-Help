---
external help file: PSScriptTools-help.xml
Module Name:
online version: https://bit.ly/33RWeAV
schema: 2.0.0
---

# New-ANSIBar

## SYNOPSIS
Display an ANSI colored bar.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-ANSIBar [-Character <String>] [-Gradient] -Range <Int32[]> [-Spacing <Int32>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-ANSIBar [-Custom <Char>] [-Gradient] -Range <Int32[]> [-Spacing <Int32>] [<CommonParameters>]
```

## DESCRIPTION
You can use this command to create colorful bars using ANSI escape sequences based on a 256 color scheme.
The default behavior is to create a gradient bar that goes from first to last values in the range and then back down again.
Or you can create a single gradient that runs from the beginning of the range to the end.
You can use one of the default characters or specify a custom one.

You can learn more about ANSI escape codes at https://en.wikipedia.org/wiki/ANSI_escape_code.

## EXAMPLES

### Example 1
```
PS C:\> New-ANSIBar -range (232..255)
```

This will create a grayscale gradient bar that goes from dark to light to dark.

### Example 2
```
PS C:\> New-ANSIBar -range (46..51) -Character BlackSquare -Spacing 3
```

### Example 3
```
PS C:\> New-ANSIBar -range (214..219) -Gradient -Spacing 5 -Character DarkShade
```

## PARAMETERS

### -Character
Specify a character to use for the bar.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:
Accepted values: FullBlock, LightShade, MediumShade, DarkShade, BlackSquare, WhiteSquare

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Custom
Specify a custom character.

```yaml
Type: Char
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Gradient
Display as a single gradient from the first value to the last.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Range
Enter a range of 256 color values, e.g.
(232..255)

```yaml
Type: Int32[]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Spacing
How many characters do you want in the bar of each value?
This will increase the overall length of the bar.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### System.String
## NOTES
* Learn more about PowerShell: http://jdhitsolutions.com/blog/essential-powershell-resources/

## RELATED LINKS

[New-RedGreenGradient]()

[Write-ANSIProgress]()

