---
external help file: ImportExcel-help.xml
Module Name: ImportExcel
online version:
schema: 2.0.0
---

# New-ExcelStyle

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
New-ExcelStyle [[-Range] <Object>] [[-NumberFormat] <Object>] [[-BorderAround] <ExcelBorderStyle>]
 [[-BorderColor] <Object>] [[-BorderBottom] <ExcelBorderStyle>] [[-BorderTop] <ExcelBorderStyle>]
 [[-BorderLeft] <ExcelBorderStyle>] [[-BorderRight] <ExcelBorderStyle>] [[-FontColor] <Object>]
 [[-Value] <Object>] [[-Formula] <Object>] [-ArrayFormula] [-ResetFont] [-Bold] [-Italic] [-Underline]
 [[-UnderLineType] <ExcelUnderLineType>] [-StrikeThru] [[-FontShift] <ExcelVerticalAlignmentFont>]
 [[-FontName] <String>] [[-FontSize] <Single>] [[-BackgroundColor] <Object>]
 [[-BackgroundPattern] <ExcelFillStyle>] [[-PatternColor] <Object>] [-WrapText]
 [[-HorizontalAlignment] <ExcelHorizontalAlignment>] [[-VerticalAlignment] <ExcelVerticalAlignment>]
 [[-TextRotation] <Int32>] [-AutoSize] [[-Width] <Single>] [[-Height] <Single>] [-Hidden] [-Locked] [-Merge]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -ArrayFormula
{{ Fill ArrayFormula Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutoSize
{{ Fill AutoSize Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: AutoFit

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
{{ Fill BackgroundColor Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 15
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundPattern
{{ Fill BackgroundPattern Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelFillStyle
Parameter Sets: (All)
Aliases:
Accepted values: None, Solid, DarkGray, MediumGray, LightGray, Gray125, Gray0625, DarkVertical, DarkHorizontal, DarkDown, DarkUp, DarkGrid, DarkTrellis, LightVertical, LightHorizontal, LightDown, LightUp, LightGrid, LightTrellis

Required: False
Position: 16
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Bold
{{ Fill Bold Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderAround
{{ Fill BorderAround Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelBorderStyle
Parameter Sets: (All)
Aliases:
Accepted values: None, Hair, Dotted, DashDot, Thin, DashDotDot, Dashed, MediumDashDotDot, MediumDashed, MediumDashDot, Thick, Medium, Double

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottom
{{ Fill BorderBottom Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelBorderStyle
Parameter Sets: (All)
Aliases:
Accepted values: None, Hair, Dotted, DashDot, Thin, DashDotDot, Dashed, MediumDashDotDot, MediumDashed, MediumDashDot, Thick, Medium, Double

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderColor
{{ Fill BorderColor Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderLeft
{{ Fill BorderLeft Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelBorderStyle
Parameter Sets: (All)
Aliases:
Accepted values: None, Hair, Dotted, DashDot, Thin, DashDotDot, Dashed, MediumDashDotDot, MediumDashed, MediumDashDot, Thick, Medium, Double

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderRight
{{ Fill BorderRight Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelBorderStyle
Parameter Sets: (All)
Aliases:
Accepted values: None, Hair, Dotted, DashDot, Thin, DashDotDot, Dashed, MediumDashDotDot, MediumDashed, MediumDashDot, Thick, Medium, Double

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderTop
{{ Fill BorderTop Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelBorderStyle
Parameter Sets: (All)
Aliases:
Accepted values: None, Hair, Dotted, DashDot, Thin, DashDotDot, Dashed, MediumDashDotDot, MediumDashed, MediumDashDot, Thick, Medium, Double

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontColor
{{ Fill FontColor Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases: ForegroundColor

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontName
{{ Fill FontName Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 13
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontShift
{{ Fill FontShift Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelVerticalAlignmentFont
Parameter Sets: (All)
Aliases:
Accepted values: None, Baseline, Subscript, Superscript

Required: False
Position: 12
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontSize
{{ Fill FontSize Description }}

```yaml
Type: System.Single
Parameter Sets: (All)
Aliases:

Required: False
Position: 14
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Formula
{{ Fill Formula Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Height
{{ Fill Height Description }}

```yaml
Type: System.Single
Parameter Sets: (All)
Aliases:

Required: False
Position: 22
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Hidden
{{ Fill Hidden Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: Hide

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HorizontalAlignment
{{ Fill HorizontalAlignment Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelHorizontalAlignment
Parameter Sets: (All)
Aliases:
Accepted values: General, Left, Center, CenterContinuous, Right, Fill, Distributed, Justify

Required: False
Position: 18
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Italic
{{ Fill Italic Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Locked
{{ Fill Locked Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Merge
{{ Fill Merge Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NumberFormat
{{ Fill NumberFormat Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases: NFormat

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PatternColor
{{ Fill PatternColor Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases: PatternColour

Required: False
Position: 17
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Range
{{ Fill Range Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases: Address

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResetFont
{{ Fill ResetFont Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StrikeThru
{{ Fill StrikeThru Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextRotation
{{ Fill TextRotation Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 20
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UnderLineType
{{ Fill UnderLineType Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelUnderLineType
Parameter Sets: (All)
Aliases:
Accepted values: None, Single, Double, SingleAccounting, DoubleAccounting

Required: False
Position: 11
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Underline
{{ Fill Underline Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value
{{ Fill Value Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VerticalAlignment
{{ Fill VerticalAlignment Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelVerticalAlignment
Parameter Sets: (All)
Aliases:
Accepted values: Top, Center, Bottom, Distributed, Justify

Required: False
Position: 19
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Width
{{ Fill Width Description }}

```yaml
Type: System.Single
Parameter Sets: (All)
Aliases:

Required: False
Position: 21
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WrapText
{{ Fill WrapText Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
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

### System.Object
## NOTES

## RELATED LINKS
