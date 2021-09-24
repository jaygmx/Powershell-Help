---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDLink.md
schema: 2.0.0
---

# New-UDMuTypography

## SYNOPSIS


## SYNTAX

### text (Default)
```
New-UDMuTypography [-Id <String>] [-Variant <String>] [-Text <String>] [-Style <Hashtable>]
 [-ClassName <String>] [-Align <String>] [-IsEndPoint] [-GutterBottom] [-NoWrap] [-IsParagraph]
 [<CommonParameters>]
```

### endpoint
```
New-UDMuTypography [-Id <String>] [-Variant <String>] [-Content <ScriptBlock>] [-Style <Hashtable>]
 [-ClassName <String>] [-Align <String>] [-IsEndPoint] [-GutterBottom] [-NoWrap] [-IsParagraph] [-AutoRefresh]
 [-RefreshInterval <Int32>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```

```



## PARAMETERS

### -Align


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: inherit, left, center, right, justify

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutoRefresh


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: endpoint
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClassName


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

### -Content


```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: endpoint
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GutterBottom


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

### -Id


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

### -IsEndPoint


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

### -IsParagraph


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

### -NoWrap


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

### -RefreshInterval


```yaml
Type: System.Int32
Parameter Sets: endpoint
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Style


```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text


```yaml
Type: System.String
Parameter Sets: text
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Variant


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: h1, h2, h3, h4, h5, h6, subtitle1, subtitle2, body1, body2, caption, button, overline, srOnly, inherit, display4, display3, display2, display1, headline, title, subheading

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
