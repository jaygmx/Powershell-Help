---
external help file: TMOutput-help.xml
Module Name: TMOutput
online version:
schema: 2.0.0
---

# Write-TMOutput

## SYNOPSIS
Sends the specified objects to the next command in the pipeline.
If the command is the last command in the pipeline, the objects are displayed in the console.

## SYNTAX

```
Write-TMOutput [[-InputObject] <PSObject[]>] [[-ForegroundColor] <String>] [[-BackgroundColor] <String>]
 [[-HorizontalPad] <Int32>] [[-VerticalPad] <Int32>] [-NoEnumerate] [<CommonParameters>]
```

## DESCRIPTION
Sends the specified objects to the next command in the pipeline.
If the command is the last command in the pipeline, the objects are displayed in the console.
This function is a wrapper for the Write-Output cmdlet with some additional features.
It allows for changing the color of the text (foreground color), and the color behind the text (background color).
It also allows for horizontal and vertical padding.

## EXAMPLES

### EXAMPLE 1
```
Write-TMOutput -InputObject 'Testing 1, 2, 3'
This example writes the text object to the console.
```

### EXAMPLE 2
```
Write-TMOutput -InputObject 'Testing 1, 2, 3' -ForegroundColor Gray -BackgroundColor Black
This example writes the text object to the console in a gray font on a black background.
```

### EXAMPLE 3
```
Write-TMOutput -InputObject 'Testing 1, 2, 3' -ForegroundColor Gray -BackgroundColor Black -HorizontalPad 10 -VerticalPad 2
This example writes the text object to the console in a gray font on a black background. It will also pad the area around the text object with the background color in both horizontal and vertical directions.
```

## PARAMETERS

### -InputObject
Specifies the objects to send down the pipeline.
Enter a variable that contains the objects, or type a command or expression that gets the objects.

```yaml
Type: System.Management.Automation.PSObject[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ForegroundColor
Specifies the text color.
The default is the current foreground color.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: [System.Console]::ForegroundColor
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
Specifies the background color.
The default is the current background color.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: [System.Console]::BackgroundColor
Accept pipeline input: False
Accept wildcard characters: False
```

### -HorizontalPad
Specifies the amount of space on each side of the included objects.
If this value doubled and added to length of the object is greater than the width of the console, it will wrap and likely cause unintended results.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -VerticalPad
Specifies the number of blank lines above and below the included objects.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoEnumerate
By default, the Write-Output cmdlet always enumerates its output.
The NoEnumerate parameter suppresses the default behavior, and prevents Write-Output from enumerating output.
The NoEnumerate parameter has no effect on collections that were created by wrapping commands in parentheses, because the parentheses force enumeration.
The Write-TMOutput function is a wrapper for Write-Output cmdlet.

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

### System.Management.Automation.PSObject
### You can pipe objects to Write-TMOutput.
## OUTPUTS

### System.Management.Automation.PSObject
### Write-TMOutput returns the objects that are submitted as input.
## NOTES
NAME: Write-TMOutput
AUTHOR: Tommy Maynard
LASTEDIT: 05/12/2016
VERSION 1.1: Removed ISE protection code; PowerShellHostName (currently) requires ConsoleHost only.
PERSONAL WEBSITE POST: http://tommymaynard.com/quick-learn-write-output-gets-foreground-and-background-colors-and-more-2016

## RELATED LINKS
