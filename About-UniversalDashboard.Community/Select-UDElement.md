---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# Select-UDElement

## SYNOPSIS
Selects an element.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Select-UDElement -ID <String> [-ScrollToElemenet] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Select-UDElement [-ToTop] [<CommonParameters>]
```

## DESCRIPTION
Selects an element, and optionally scrolls to it.

## EXAMPLES

### Example 1
```
PS C:\> Select-UDElement -Id 'textbox' -ScrollToElement
```

Selects the text box with the ID 'textbox' and scrolls to the position on page.

### Example 2
```
PS C:\> Select-UDElement -ToTop
```

Scrolls the page to the top.

## PARAMETERS

### -ID
The ID of the element to select.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScrollToElemenet
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ToTop
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: False
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
