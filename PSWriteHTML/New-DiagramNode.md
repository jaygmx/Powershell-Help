---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-DiagramNode

## SYNOPSIS
Creates nodes on a diagram

## SYNTAX

### Shape (Default)
```
New-DiagramNode [-HtmlTextBox <ScriptBlock>] [-Id <String>] [-Label <String>] [-Title <String>]
 [-To <String[]>] [-ArrowsToEnabled] [-ArrowsMiddleEnabled] [-ArrowsFromEnabled] [-LinkColor <String>]
 [-Shape <String>] [-BorderWidth <Int32>] [-BorderWidthSelected <Int32>] [-Chosen <Boolean>]
 [-ColorBorder <String>] [-ColorBackground <String>] [-ColorHighlightBorder <String>]
 [-ColorHighlightBackground <String>] [-ColorHoverBorder <String>] [-ColorHoverBackground <String>]
 [-FixedX <Boolean>] [-FixedY <Boolean>] [-FontColor <String>] [-FontSize <Int32>] [-FontName <String>]
 [-FontBackground <String>] [-FontStrokeWidth <Int32>] [-FontStrokeColor <String>] [-FontAlign <String>]
 [-FontMulti <String>] [-FontVAdjust <Int32>] [-Size <Int32>] [-X <Int32>] [-Y <Int32>] [-Level <Int32>]
 [-HeightConstraintMinimum <Int32>] [-HeightConstraintVAlign <String>] [-WidthConstraintMinimum <Int32>]
 [-WidthConstraintMaximum <Int32>] [<CommonParameters>]
```

### Image
```
New-DiagramNode [-HtmlTextBox <ScriptBlock>] [-Id <String>] [-Label <String>] [-Title <String>]
 [-To <String[]>] [-ArrowsToEnabled] [-ArrowsMiddleEnabled] [-ArrowsFromEnabled] [-LinkColor <String>]
 [-ImageType <String>] [-Image <Uri>] [-BorderWidth <Int32>] [-BorderWidthSelected <Int32>]
 [-BrokenImages <String>] [-Chosen <Boolean>] [-ColorBorder <String>] [-ColorBackground <String>]
 [-ColorHighlightBorder <String>] [-ColorHighlightBackground <String>] [-ColorHoverBorder <String>]
 [-ColorHoverBackground <String>] [-FixedX <Boolean>] [-FixedY <Boolean>] [-FontColor <String>]
 [-FontSize <Int32>] [-FontName <String>] [-FontBackground <String>] [-FontStrokeWidth <Int32>]
 [-FontStrokeColor <String>] [-FontAlign <String>] [-FontMulti <String>] [-FontVAdjust <Int32>] [-Size <Int32>]
 [-X <Int32>] [-Y <Int32>] [-Level <Int32>] [-HeightConstraintMinimum <Int32>]
 [-HeightConstraintVAlign <String>] [-WidthConstraintMinimum <Int32>] [-WidthConstraintMaximum <Int32>]
 [<CommonParameters>]
```

### FontAwesomeSolid
```
New-DiagramNode [-HtmlTextBox <ScriptBlock>] [-Id <String>] [-Label <String>] [-Title <String>]
 [-To <String[]>] [-ArrowsToEnabled] [-ArrowsMiddleEnabled] [-ArrowsFromEnabled] [-LinkColor <String>]
 [-BorderWidth <Int32>] [-BorderWidthSelected <Int32>] [-Chosen <Boolean>] [-FixedX <Boolean>]
 [-FixedY <Boolean>] [-FontColor <String>] [-FontSize <Int32>] [-FontName <String>] [-FontBackground <String>]
 [-FontStrokeWidth <Int32>] [-FontStrokeColor <String>] [-FontAlign <String>] [-FontMulti <String>]
 [-FontVAdjust <Int32>] [-Size <Int32>] [-X <Int32>] [-Y <Int32>] [-IconAsImage] [-IconColor <String>]
 [-IconSolid <String>] [-Level <Int32>] [-HeightConstraintMinimum <Int32>] [-HeightConstraintVAlign <String>]
 [-WidthConstraintMinimum <Int32>] [-WidthConstraintMaximum <Int32>] [<CommonParameters>]
```

### FontAwesomeRegular
```
New-DiagramNode [-HtmlTextBox <ScriptBlock>] [-Id <String>] [-Label <String>] [-Title <String>]
 [-To <String[]>] [-ArrowsToEnabled] [-ArrowsMiddleEnabled] [-ArrowsFromEnabled] [-LinkColor <String>]
 [-BorderWidth <Int32>] [-BorderWidthSelected <Int32>] [-Chosen <Boolean>] [-FixedX <Boolean>]
 [-FixedY <Boolean>] [-FontColor <String>] [-FontSize <Int32>] [-FontName <String>] [-FontBackground <String>]
 [-FontStrokeWidth <Int32>] [-FontStrokeColor <String>] [-FontAlign <String>] [-FontMulti <String>]
 [-FontVAdjust <Int32>] [-Size <Int32>] [-X <Int32>] [-Y <Int32>] [-IconAsImage] [-IconColor <String>]
 [-IconRegular <String>] [-Level <Int32>] [-HeightConstraintMinimum <Int32>] [-HeightConstraintVAlign <String>]
 [-WidthConstraintMinimum <Int32>] [-WidthConstraintMaximum <Int32>] [<CommonParameters>]
```

### FontAwesomeBrands
```
New-DiagramNode [-HtmlTextBox <ScriptBlock>] [-Id <String>] [-Label <String>] [-Title <String>]
 [-To <String[]>] [-ArrowsToEnabled] [-ArrowsMiddleEnabled] [-ArrowsFromEnabled] [-LinkColor <String>]
 [-BorderWidth <Int32>] [-BorderWidthSelected <Int32>] [-Chosen <Boolean>] [-FixedX <Boolean>]
 [-FixedY <Boolean>] [-FontColor <String>] [-FontSize <Int32>] [-FontName <String>] [-FontBackground <String>]
 [-FontStrokeWidth <Int32>] [-FontStrokeColor <String>] [-FontAlign <String>] [-FontMulti <String>]
 [-FontVAdjust <Int32>] [-Size <Int32>] [-X <Int32>] [-Y <Int32>] [-IconAsImage] [-IconColor <String>]
 [-IconBrands <String>] [-Level <Int32>] [-HeightConstraintMinimum <Int32>] [-HeightConstraintVAlign <String>]
 [-WidthConstraintMinimum <Int32>] [-WidthConstraintMaximum <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Creates nodes on a diagram

## EXAMPLES

### EXAMPLE 1
```
An example
```

## PARAMETERS

### -HtmlTextBox
Experimental TextBox to put HTML instead of Image using SVG

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Id of a node.
If not set, label will be used as Id.

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

### -Label
Label for a diagram

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

### -Title
Label that shows up when hovering over node

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

### -To
Parameter description

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ArrowsToEnabled
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

### -ArrowsMiddleEnabled
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

### -ArrowsFromEnabled
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

### -LinkColor
Parameter description

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: EdgeColor

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Shape
Parameter description

```yaml
Type: System.String
Parameter Sets: Shape
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ImageType
Parameter description

```yaml
Type: System.String
Parameter Sets: Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Image
Parameter description

```yaml
Type: System.Uri
Parameter Sets: Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderWidth
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderWidthSelected
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BrokenImages
Parameter description

```yaml
Type: System.String
Parameter Sets: Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Chosen
Parameter description

```yaml
Type: System.Nullable`1[System.Boolean]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColorBorder
Parameter description

```yaml
Type: System.String
Parameter Sets: Shape, Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColorBackground
Parameter description

```yaml
Type: System.String
Parameter Sets: Shape, Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColorHighlightBorder
Parameter description

```yaml
Type: System.String
Parameter Sets: Shape, Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColorHighlightBackground
Parameter description

```yaml
Type: System.String
Parameter Sets: Shape, Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColorHoverBorder
Parameter description

```yaml
Type: System.String
Parameter Sets: Shape, Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColorHoverBackground
Parameter description

```yaml
Type: System.String
Parameter Sets: Shape, Image
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FixedX
Parameter description

```yaml
Type: System.Nullable`1[System.Boolean]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FixedY
Parameter description

```yaml
Type: System.Nullable`1[System.Boolean]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontColor
Color of the label text.

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

### -FontSize
Size of the label text.

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontName
Font face (or font family) of the label text.

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

### -FontBackground
When not undefined but a color string, a background rectangle will be drawn behind the label in the supplied color.

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

### -FontStrokeWidth
As an alternative to the background rectangle, a stroke can be drawn around the text.
When a value higher than 0 is supplied, the stroke will be draw

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontStrokeColor
This is the color of the stroke assuming the value for stroke is higher than 0.

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

### -FontAlign
This can be set to 'left' to make the label left-aligned.
Otherwise, defaults to 'center'.

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

### -FontMulti
If false, the label is treated as pure text drawn with the base font.
If true or 'html' the label may be multifonted, with bold, italic and code markup, interpreted as html.
If the value is 'markdown' or 'md' the label may be multifonted, with bold, italic and code markup, interpreted as markdown.
The bold, italic, bold-italic and monospaced fonts may be set up under in the font.bold, font.ital, font.boldital and font.mono properties, respectively.

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

### -FontVAdjust
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Size
The size is used to determine the size of node shapes that do not have the label inside of them.
These shapes are: image, circularImage, diamond, dot, star, triangle, triangleDown, hexagon, square and icon

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -X
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Y
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconAsImage
Parameter description

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontAwesomeSolid, FontAwesomeRegular, FontAwesomeBrands
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconColor
Parameter description

```yaml
Type: System.String
Parameter Sets: FontAwesomeSolid, FontAwesomeRegular, FontAwesomeBrands
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconBrands
Parameter description

```yaml
Type: System.String
Parameter Sets: FontAwesomeBrands
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconRegular
Parameter description

```yaml
Type: System.String
Parameter Sets: FontAwesomeRegular
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconSolid
Parameter description

```yaml
Type: System.String
Parameter Sets: FontAwesomeSolid
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Level
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeightConstraintMinimum
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeightConstraintVAlign
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

### -WidthConstraintMinimum
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WidthConstraintMaximum
Parameter description

```yaml
Type: System.Nullable`1[System.Int32]
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
