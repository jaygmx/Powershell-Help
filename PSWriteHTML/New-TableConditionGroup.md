---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-TableConditionGroup

## SYNOPSIS


## SYNTAX

```
New-TableConditionGroup [[-Conditions] <ScriptBlock>] [[-Logic] <String>] [[-HighlightHeaders] <String[]>]
 [-Row] [-Inline] [[-Color] <String>] [[-BackgroundColor] <String>] [[-FontSize] <Int32>]
 [[-FontWeight] <String>] [[-FontStyle] <String>] [[-FontVariant] <String>] [[-FontFamily] <String>]
 [[-Alignment] <String>] [[-TextDecoration] <String>] [[-TextTransform] <String>] [[-Direction] <String>]
 [[-FailColor] <String>] [[-FailBackgroundColor] <String>] [[-FailFontSize] <Object>]
 [[-FailFontWeight] <String>] [[-FailFontStyle] <String>] [[-FailFontVariant] <String>]
 [[-FailFontFamily] <String>] [[-FailAlignment] <String>] [[-FailTextDecoration] <String>]
 [[-FailTextTransform] <String>] [[-FailDirection] <String>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Alignment


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: left, center, right, justify

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Conditions


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
Accepted values: rtl

Required: False
Position: 13
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailAlignment


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: left, center, right, justify

Required: False
Position: 21
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailBackgroundColor


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 15
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailColor


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 14
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailDirection


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: rtl

Required: False
Position: 24
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailFontFamily


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

### -FailFontSize


```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 16
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailFontStyle


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, italic, oblique

Required: False
Position: 18
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailFontVariant


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, small-caps

Required: False
Position: 19
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailFontWeight


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, bold, bolder, lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900

Required: False
Position: 17
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailTextDecoration


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: none, line-through, overline, underline

Required: False
Position: 22
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FailTextTransform


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: uppercase, lowercase, capitalize

Required: False
Position: 23
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontFamily


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

### -FontSize


```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontStyle


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, italic, oblique

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontVariant


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, small-caps

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontWeight


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: normal, bold, bolder, lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HighlightHeaders


```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Inline


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

### -Logic


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: AND, OR, NONE

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Row


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

### -TextDecoration


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: none, line-through, overline, underline

Required: False
Position: 11
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextTransform


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: uppercase, lowercase, capitalize

Required: False
Position: 12
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
