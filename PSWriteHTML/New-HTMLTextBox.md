---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLTextBox

## SYNOPSIS
Adds text to HTML where each line in TextBlock is treated as next line (adds BR to each line)

## SYNTAX

```
New-HTMLTextBox [[-TextBlock] <ScriptBlock>] [-Color <String[]>] [-BackGroundColor <String[]>]
 [-FontSize <Int32[]>] [-FontWeight <String[]>] [-FontStyle <String[]>] [-TextDecoration <String[]>]
 [-FontVariant <String[]>] [-FontFamily <String[]>] [-Alignment <String[]>] [-TextTransform <String[]>]
 [-Direction <String[]>] [-LineBreak] [<CommonParameters>]
```

## DESCRIPTION
Adds text to HTML where each line in TextBlock is treated as next line (adds BR to each line).
Automatic line breaks are main feature that differentiate New-HTMLTextBox from New-HTMLText
where TextBlock is treated as single line of text unless LineBreak switch is used.

## EXAMPLES

### EXAMPLE 1
```
New-HTMLTextBox {
    "Hello $UserNotify,"
    ""
    "Your password is due to expire in $PasswordExpiryDays days."
    ""
    'To change your password: '
    '- press CTRL+ALT+DEL -> Change a password...'
    ''
    'If you have forgotten your password and need to reset it, you can do this by clicking here. '
    "In case of problems please contact the HelpDesk by visiting [Evotec Website](https://evotec.xyz) or by sending an email to Help Desk."
    ''
    'Alternatively you can always call Help Desk at +48 22 00 00 00'
    ''
    'Kind regards,'
    'Evotec IT'
}
```

## PARAMETERS

### -TextBlock
ScriptBlock of one or more strings

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color
Color of Text to set.
Choose one or more colors from up to 800 defined colors.
Alternatively provide your own Hex value

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackGroundColor
Color of Background for a Text to set.
Choose one or more colors from up to 800 defined colors.
Alternatively provide your own Hex value

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontSize
Choose FontSize.
You can provide just int value which will assume pixels or string value with any other size value.

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases: Size

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontWeight
Parameter description

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontStyle
Parameter description

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextDecoration
Parameter description

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontVariant
Parameter description

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontFamily
Parameter description

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -Alignment
Chhoose Alignment

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextTransform
Parameter description

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -Direction
Parameter description

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -LineBreak
Parameter description

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
General notes

## RELATED LINKS
