---
external help file: PSWriteColor-help.xml
Module Name: PSWriteColor
online version:
schema: 2.0.0
---

# Write-Color

## SYNOPSIS
Write-Color is a wrapper around Write-Host.

It provides:
- Easy manipulation of colors,
- Logging output to file (log)
- Nice formatting options out of the box.

## SYNTAX

```
Write-Color [[-Text] <String[]>] [[-Color] <ConsoleColor[]>] [[-BackGroundColor] <ConsoleColor[]>]
 [[-StartTab] <Int32>] [[-LinesBefore] <Int32>] [[-LinesAfter] <Int32>] [[-StartSpaces] <Int32>]
 [[-LogFile] <String>] [[-DateTimeFormat] <String>] [[-LogTime] <Boolean>] [[-LogRetry] <Int32>]
 [[-Encoding] <String>] [-ShowTime] [-NoNewLine] [<CommonParameters>]
```

## DESCRIPTION
Author: przemyslaw.klys at evotec.pl
Project website: https://evotec.xyz/hub/scripts/write-color-ps1/
Project support: https://github.com/EvotecIT/PSWriteColor

Original idea: Josh (https://stackoverflow.com/users/81769/josh)

## EXAMPLES

### EXAMPLE 1
```
Write-Color -Text "Red ", "Green ", "Yellow " -Color Red,Green,Yellow
```

### EXAMPLE 2
```
Write-Color -Text "This is text in Green ",
				"followed by red ",
				"and then we have Magenta... ",
				"isn't it fun? ",
				"Here goes DarkCyan" -Color Green,Red,Magenta,White,DarkCyan
```

### EXAMPLE 3
```
Write-Color -Text "This is text in Green ",
				"followed by red ",
				"and then we have Magenta... ",
				"isn't it fun? ",
                   "Here goes DarkCyan" -Color Green,Red,Magenta,White,DarkCyan -StartTab 3 -LinesBefore 1 -LinesAfter 1
```

### EXAMPLE 4
```
Write-Color "1. ", "Option 1" -Color Yellow, Green
Write-Color "2. ", "Option 2" -Color Yellow, Green
Write-Color "3. ", "Option 3" -Color Yellow, Green
Write-Color "4. ", "Option 4" -Color Yellow, Green
Write-Color "9. ", "Press 9 to exit" -Color Yellow, Gray -LinesBefore 1
```

### EXAMPLE 5
```
Write-Color -LinesBefore 2 -Text "This little ","message is ", "written to log ", "file as well." `
			-Color Yellow, White, Green, Red, Red -LogFile "C:\testing.txt" -TimeFormat "yyyy-MM-dd HH:mm:ss"
Write-Color -Text "This can get ","handy if ", "want to display things, and log actions to file ", "at the same time." `
			-Color Yellow, White, Green, Red, Red -LogFile "C:\testing.txt"
```

### EXAMPLE 6
```
# Added in 0.5
Write-Color -T "My text", " is ", "all colorful" -C Yellow, Red, Green -B Green, Green, Yellow
wc -t "my text" -c yellow -b green
wc -text "my text" -c red
```

## PARAMETERS

### -Text
{{ Fill Text Description }}

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: T

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color
{{ Fill Color Description }}

```yaml
Type: System.ConsoleColor[]
Parameter Sets: (All)
Aliases: C, ForegroundColor, FGC
Accepted values: Black, DarkBlue, DarkGreen, DarkCyan, DarkRed, DarkMagenta, DarkYellow, Gray, DarkGray, Blue, Green, Cyan, Red, Magenta, Yellow, White

Required: False
Position: 2
Default value: White
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackGroundColor
{{ Fill BackGroundColor Description }}

```yaml
Type: System.ConsoleColor[]
Parameter Sets: (All)
Aliases: B, BGC
Accepted values: Black, DarkBlue, DarkGreen, DarkCyan, DarkRed, DarkMagenta, DarkYellow, Gray, DarkGray, Blue, Green, Cyan, Red, Magenta, Yellow, White

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartTab
{{ Fill StartTab Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases: Indent

Required: False
Position: 4
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -LinesBefore
{{ Fill LinesBefore Description }}

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

### -LinesAfter
{{ Fill LinesAfter Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartSpaces
{{ Fill StartSpaces Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -LogFile
{{ Fill LogFile Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: L

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DateTimeFormat
{{ Fill DateTimeFormat Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: DateFormat, TimeFormat

Required: False
Position: 9
Default value: Yyyy-MM-dd HH:mm:ss
Accept pipeline input: False
Accept wildcard characters: False
```

### -LogTime
{{ Fill LogTime Description }}

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases: LogTimeStamp

Required: False
Position: 10
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
```

### -LogRetry
{{ Fill LogRetry Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 11
Default value: 2
Accept pipeline input: False
Accept wildcard characters: False
```

### -Encoding
{{ Fill Encoding Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 12
Default value: Unicode
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShowTime
{{ Fill ShowTime Description }}

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

### -NoNewLine
{{ Fill NoNewLine Description }}

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

## NOTES
Additional Notes:
- TimeFormat https://msdn.microsoft.com/en-us/library/8kb3ddd4.aspx

## RELATED LINKS
