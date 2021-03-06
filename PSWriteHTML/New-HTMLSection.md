---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLSection

## SYNOPSIS


## SYNTAX

```
New-HTMLSection [[-Content] <ScriptBlock>] [-HeaderText <String>] [-HeaderTextColor <String>]
 [-HeaderTextSize <String>] [-HeaderTextAlignment <String>] [-HeaderBackGroundColor <String>]
 [-BackgroundColor <String>] [-CanCollapse] [-IsHidden] [-Collapsed] [-Height <Object>] [-Width <Object>]
 [-Invisible] [-Wrap <String>] [-Direction <String>] [-AlignContent <String>] [-AlignItems <String>]
 [-JustifyContent <String>] [-BorderRadius <String>] [-AnchorName <String>]
 [-StyleSheetsConfiguration <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

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

### -AnchorName


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


```yaml
Type: System.String
Parameter Sets: (All)
Aliases: BackgroundShade

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderRadius


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: 0px, 5px, 10px, 15px, 20px, 25px

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CanCollapse


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: Collapsable

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Collapsed


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

### -Content


```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
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

### -HeaderBackGroundColor


```yaml
Type: System.String
Parameter Sets: (All)
Aliases: TextBackGroundColor

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeaderText


```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Name, Title

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeaderTextAlignment


```yaml
Type: System.String
Parameter Sets: (All)
Aliases: TextAlignment
Accepted values: center, left, right, justify

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeaderTextColor


```yaml
Type: System.String
Parameter Sets: (All)
Aliases: TextColor

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeaderTextSize


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

### -Height


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

### -Invisible


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

### -IsHidden


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

### -StyleSheetsConfiguration


```yaml
Type: System.Collections.IDictionary
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Width


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
