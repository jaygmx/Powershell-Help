---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLTableStyle

## SYNOPSIS
Apply new style for HTML Table

## SYNTAX

```
New-HTMLTableStyle [-Type <String>] [-FontSize <String>] [-FontWeight <String>] [-FontStyle <String>]
 [-FontVariant <String>] [-FontFamily <String>] [-BackgroundColor <String>] [-TextColor <String>]
 [-TextDecoration <String>] [-TextTransform <String>] [-TextAlign <String>] [-BorderTopStyle <Object>]
 [-BorderTopColor <String>] [-BorderTopWidthSize <String>] [-BorderBottomStyle <Object>]
 [-BorderBottomColor <String>] [-BorderBottomWidthSize <String>] [-BorderLeftStyle <Object>]
 [-BorderLeftColor <String>] [-BorderLeftWidthSize <String>] [-BorderRightStyle <Object>]
 [-BorderRightColor <String>] [-BorderRightWidthSize <String>] [<CommonParameters>]
```

## DESCRIPTION
Apply new style for HTML Table.
Currently only works with DataTables.

## EXAMPLES

### EXAMPLE 1
```
$Table = Get-Process | Select-Object -First 3
New-HTML -ShowHTML -HtmlData {
    New-HTMLTable -DataTable $table -HideButtons {
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor Yellow -TextColor Aquamarine -TextAlign center -Type RowOdd
        New-HTMLTableStyle -BackgroundColor Red -TextColor Aquamarine -Type Button
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor DarkSlateGray -TextColor Aquamarine -TextAlign center -Type RowEven
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor DarkSlateGray -TextColor Aquamarine -TextAlign center -Type Row
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor DarkSlateGray -TextColor Aquamarine -TextAlign center -Type Header
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor Orange -TextColor Aquamarine -TextAlign center -Type Footer
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor Orange -TextColor Aquamarine -TextAlign center -Type RowSelectedEven
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor Green -TextColor Aquamarine -TextAlign center -Type RowSelectedOdd
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor Yellow -TextColor Aquamarine -TextAlign center -Type RowHover
        New-HTMLTableStyle -FontFamily 'Calibri' -BackgroundColor Red -TextColor Aquamarine -TextAlign center -Type RowHoverSelected
        New-HTMLTableStyle -Type Header -BorderLeftStyle dashed -BorderLeftColor Red -BorderLeftWidthSize 1px
        New-HTMLTableStyle -Type Footer -BorderLeftStyle dotted -BorderLeftColor Red -BorderleftWidthSize 1px
        New-HTMLTableStyle -Type Footer -BorderTopStyle none -BorderTopColor Red -BorderTopWidthSize 5px -BorderBottomColor Yellow -BorderBottomStyle solid
        New-HTMLTableStyle -Type Footer -BorderTopStyle none -BorderTopColor Red -BorderTopWidthSize 5px -BorderBottomColor Yellow -BorderBottomStyle solid
        New-HTMLTableStyle -Type Footer -BorderTopStyle none -BorderTopColor Red -BorderTopWidthSize 5px -BorderBottomColor Yellow -BorderBottomStyle none
    } -DisablePaging
} -FilePath $PSScriptRoot\Example7_TableStyle.html -Online
```

## PARAMETERS

### -Type
Choose type to apply style on.
You can choose from: 'Content', 'Table', 'Header', 'Row', 'Footer', 'RowOdd', 'RowEven', 'RowSelected', 'RowSelectedEven', 'RowSelectedOdd', 'RowHover', 'RowHoverSelected', 'Button'.
Content is duplicate to Row.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Table
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontSize
Choose FontSize

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: TextSize

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontWeight
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontStyle
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontVariant
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontFamily
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextColor
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextDecoration
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextTransform
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextAlign
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: FontAlign, Align

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderTopStyle
Parameter description

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderTopColor
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderTopWidthSize
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomStyle
Parameter description

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomColor
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderBottomWidthSize
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderLeftStyle
Parameter description

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderLeftColor
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderLeftWidthSize
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderRightStyle
Parameter description

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderRightColor
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderRightWidthSize
Parameter description

```yaml
Type: System.String
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

## OUTPUTS

## NOTES
General notes

## RELATED LINKS
