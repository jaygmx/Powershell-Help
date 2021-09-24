---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLChart

## SYNOPSIS


## SYNTAX

```
New-HTMLChart [[-ChartSettings] <ScriptBlock>] [[-Title] <String>] [[-TitleAlignment] <String>]
 [[-TitleMargin] <Int32>] [[-TitleOffsetX] <Int32>] [[-TitleOffsetY] <Int32>] [[-TitleFloating] <Int32>]
 [[-TitleFontSize] <Object>] [[-TitleFontWeight] <String>] [[-TitleFontFamily] <String>]
 [[-TitleColor] <String>] [[-SubTitle] <String>] [[-SubTitleAlignment] <String>] [[-SubTitleMargin] <Int32>]
 [[-SubTitleOffsetX] <Int32>] [[-SubTitleOffsetY] <Int32>] [[-SubTitleFloating] <Int32>]
 [[-SubTitleFontSize] <Object>] [[-SubTitleFontWeight] <String>] [[-SubTitleFontFamily] <String>]
 [[-SubTitleColor] <String>] [[-Height] <Object>] [[-Width] <Object>] [-Gradient] [-Patterned] [[-Id] <String>]
 [[-Group] <String>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -ChartSettings


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

### -Gradient


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: GradientColors

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Group


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 24
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
Position: 21
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 23
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Patterned


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: PatternedColors

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitle


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 11
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleAlignment


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: center, left, right

Required: False
Position: 12
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleColor


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 20
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleFloating


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 16
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleFontFamily


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 19
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleFontSize


```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 17
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleFontWeight


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, bold, bolder, lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900

Required: False
Position: 18
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleMargin


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 13
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleOffsetX


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 14
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubTitleOffsetY


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 15
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Title


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleAlignment


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: center, left, right

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleColor


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleFloating


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleFontFamily


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleFontSize


```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleFontWeight


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, bold, bolder, lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleMargin


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleOffsetX


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleOffsetY


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
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
Position: 22
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
