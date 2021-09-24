---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# Invoke-UDEvent

## SYNOPSIS
Performs a clientside "click" event on the specified id, if the element is clickable.

## SYNTAX

### onClick
```
Invoke-UDEvent [-Id] <String> [-event] <String> [<CommonParameters>]
```

### Scheduled
```
Invoke-UDEvent [-Id] <String> [-scheduled] [<CommonParameters>]
```

## DESCRIPTION
Performs a clientside "click" event on the specified id, if the element is clickable.

## EXAMPLES

### Example 1
```
PS C:\> Invoke-UDEvent -id "someid" -event "onClick"
```

Performs a clientside "click" event on the specified id, if the element is clickable.

## PARAMETERS

### -event
The typeof event to trigger

```yaml
Type: System.String
Parameter Sets: onClick
Aliases:
Accepted values: onClick

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The id of the event to trigger.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -scheduled


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Scheduled
Aliases:

Required: True
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
