---
external help file: UniversalDashboard.dll-Help.xml
Module Name: UniversalDashboard.Community
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# Select-UDElement

## SYNOPSIS
Selects an element.

## SYNTAX

### Normal
```
Select-UDElement -ID <String> [-ScrollToElement] [<CommonParameters>]
```

### ToTop
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
Type: System.String
Parameter Sets: Normal
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ToTop
@{Text=}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ToTop
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScrollToElement


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Normal
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

## RELATED LINKS
