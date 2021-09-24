---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLTabStyle

## SYNOPSIS


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

```



## PARAMETERS

### -Align


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
