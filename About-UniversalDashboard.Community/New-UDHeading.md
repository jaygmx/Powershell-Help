---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDHeading.md
schema: 2.0.0
---

# New-UDHeading

## SYNOPSIS
Creates a heading.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDHeading [-Color <DashboardColor>] [-Content <ScriptBlock>] [-Id <String>] [-Size <Object>]
 [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDHeading [-Color <DashboardColor>] [-Id <String>] [-Size <Object>] [-Text <String>] [<CommonParameters>]
```

## DESCRIPTION
Creates a heading.

## EXAMPLES

### Heading
```
New-UDHeading -Size 3 -Content { "Header" }
```

Creates the heading "Header" with a size of 3.

## PARAMETERS

### -Color
Font color for the heading.

```yaml
Type: DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Content
Content for the heading.

```yaml
Type: ScriptBlock
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The ID of this heading.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Size
Size of this heading from 1 to 6.
1 is the largest and 6 is the smallest.

```yaml
Type: Object
Parameter Sets: (All)
Aliases:
Accepted values: 1, 2, 3, 4, 5, 6

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text


```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
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
*

## RELATED LINKS
