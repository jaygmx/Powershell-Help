---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLCalendar

## SYNOPSIS


## SYNTAX

```
New-HTMLCalendar [[-CalendarSettings] <ScriptBlock>] [[-HeaderLeft] <String[]>] [[-HeaderCenter] <String[]>]
 [[-HeaderRight] <String[]>] [[-DefaultDate] <DateTime>] [[-NavigationLinks] <Boolean>]
 [[-NowIndicator] <Boolean>] [[-EventLimit] <Boolean>] [[-WeekNumbers] <Boolean>] [[-Selectable] <Boolean>]
 [[-SelectMirror] <Boolean>] [-BusinessHours] [-Editable] [[-InitialView] <String>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -BusinessHours


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

### -CalendarSettings


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

### -DefaultDate


```yaml
Type: System.DateTime
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Editable


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

### -EventLimit


```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeaderCenter


```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:
Accepted values: prev, next, today, prevYear, nextYear, dayGridDay, dayGridWeek, dayGridMonth, timeGridWeek, timeGridDay, listDay, listWeek, listMonth, title

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeaderLeft


```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:
Accepted values: prev, next, today, prevYear, nextYear, dayGridDay, dayGridWeek, dayGridMonth, timeGridWeek, timeGridDay, listDay, listWeek, listMonth, title

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeaderRight


```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:
Accepted values: prev, next, today, prevYear, nextYear, dayGridDay, dayGridWeek, dayGridMonth, timeGridWeek, timeGridDay, listDay, listWeek, listMonth, title

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InitialView


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: dayGridDay, dayGridWeek, dayGridMonth, timeGridDay, timeGridWeek, listDay, listWeek, listMonth

Required: False
Position: 11
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NavigationLinks


```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NowIndicator


```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SelectMirror


```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Selectable


```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WeekNumbers


```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
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
