---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLTabStyle

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### Manual (Default)
```
New-HTMLTabStyle [-FontSize <String>] [-FontSizeActive <String>] [-TextColor <String>]
 [-TextColorActive <String>] [-FontWeight <String>] [-FontWeightActive <String>] [-FontStyle <String>]
 [-FontStyleActive <String>] [-FontVariant <String>] [-FontVariantActive <String>] [-FontFamily <String>]
 [-FontFamilyActive <String>] [-TextDecoration <String>] [-TextDecorationActive <String>]
 [-BackgroundColor <String>] [-BackgroundColorActive <String>] [-BackgroundColorActiveTarget <String>]
 [-BorderRadius <String>] [-TextTransform <String>] [-TextTransformActive <String>] [-SlimTabs] [-Transition]
 [-LinearGradient] [-RemoveShadow] [-BorderStyle <String>] [-BorderColor <String>]
 [-BorderBottomWidth <String>] [-BorderBottomStyle <String>] [-BorderBottomColor <String>]
 [-BorderBottomWidthActive <String>] [-BorderBottomStyleActive <String>] [-BorderBottomColorActive <String>]
 [-Align <String>] [-Wrap <String>] [-Direction <String>] [-AlignContent <String>] [-AlignItems <String>]
 [-JustifyContent <String>] [-RowElements <Int32>] [<CommonParameters>]
```

### Styled
```
New-HTMLTabStyle [-Style <String>] [-Align <String>] [-Wrap <String>] [-Direction <String>]
 [-AlignContent <String>] [-AlignItems <String>] [-JustifyContent <String>] [-RowElements <Int32>]
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

### -Align
{{ Fill Align Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: AlignTabs
Accepted values: left, right, center, justify

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlignContent
{{ Fill AlignContent Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: flex-start, flex-end, center, space-between, space-around, stretch

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlignItems
{{ Fill AlignItems Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: stretch, flex-start, flex-end, center, baseline

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
{{ Fill BackgroundColor Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColorActive
{{ Fill BackgroundColorActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases: SelectorColor

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColorActiveTarget
{{ Fill BackgroundColorActiveTarget Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases: SelectorColorTarget

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomColor
{{ Fill BorderBottomColor Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomColorActive
{{ Fill BorderBottomColorActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomStyle
{{ Fill BorderBottomStyle Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: none, hidden, dotted, dashed, solid, double, groove, ridge, inset, outset

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomStyleActive
{{ Fill BorderBottomStyleActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: none, hidden, dotted, dashed, solid, double, groove, ridge, inset, outset

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomWidth
{{ Fill BorderBottomWidth Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: medium, thin, thick

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomWidthActive
{{ Fill BorderBottomWidthActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: medium, thin, thick

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderColor
{{ Fill BorderColor Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderRadius
{{ Fill BorderRadius Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: 0px, 5px, 10px, 15px, 20px, 25px

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderStyle
{{ Fill BorderStyle Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: none, hidden, dotted, dashed, solid, double, groove, ridge, inset, outset

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Direction
{{ Fill Direction Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: row, row-reverse, column, column-reverse

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontFamily
{{ Fill FontFamily Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontFamilyActive
{{ Fill FontFamilyActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontSize
{{ Fill FontSize Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases: TextSize

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontSizeActive
{{ Fill FontSizeActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases: TextSizeActive

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontStyle
{{ Fill FontStyle Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: normal, italic, oblique

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontStyleActive
{{ Fill FontStyleActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: normal, italic, oblique

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontVariant
{{ Fill FontVariant Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: normal, small-caps

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontVariantActive
{{ Fill FontVariantActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: normal, small-caps

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontWeight
{{ Fill FontWeight Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: normal, bold, bolder, lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontWeightActive
{{ Fill FontWeightActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: normal, bold, bolder, lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JustifyContent
{{ Fill JustifyContent Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: flex-start, flex-end, center

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LinearGradient
{{ Fill LinearGradient Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveShadow
{{ Fill RemoveShadow Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RowElements
{{ Fill RowElements Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SlimTabs
{{ Fill SlimTabs Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Style
{{ Fill Style Description }}

```yaml
Type: System.String
Parameter Sets: Styled
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextColor
{{ Fill TextColor Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextColorActive
{{ Fill TextColorActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextDecoration
{{ Fill TextDecoration Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: none, line-through, overline, underline

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextDecorationActive
{{ Fill TextDecorationActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: none, line-through, overline, underline

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextTransform
{{ Fill TextTransform Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: uppercase, lowercase, capitalize

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextTransformActive
{{ Fill TextTransformActive Description }}

```yaml
Type: System.String
Parameter Sets: Manual
Aliases:
Accepted values: uppercase, lowercase, capitalize

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Transition
{{ Fill Transition Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Manual
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Wrap
{{ Fill Wrap Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: wrap, nowrap, wrap-reverse

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
