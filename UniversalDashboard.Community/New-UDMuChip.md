---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDLink.md
schema: 2.0.0
---

# New-UDMuChip

## SYNOPSIS


## SYNTAX

### Icon (Default)
```
New-UDMuChip [-Id <String>] [[-Label] <String>] [[-OnDelete] <Object>] [[-OnClick] <Object>] [[-Icon] <Object>]
 [[-Style] <Hashtable>] [[-Variant] <String>] [-Clickable] [<CommonParameters>]
```

### Avatar
```
New-UDMuChip [-Id <String>] [[-Label] <String>] [[-OnDelete] <Object>] [[-OnClick] <Object>]
 [[-Style] <Hashtable>] [[-Variant] <String>] [-Clickable] [[-Avatar] <String>] [[-AvatarType] <String>]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```

```



## PARAMETERS

### -Avatar


```yaml
Type: System.String
Parameter Sets: Avatar
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AvatarType


```yaml
Type: System.String
Parameter Sets: Avatar
Aliases:
Accepted values: letter, image

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Clickable


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Icon


```yaml
Type: System.Object
Parameter Sets: Icon
Aliases:

Required: False
Position: 1
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
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Label


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OnClick


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

### -OnDelete


```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
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
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Variant


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: outlined, default

Required: False
Position: 3
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
