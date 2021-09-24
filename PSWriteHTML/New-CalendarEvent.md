---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-CalendarEvent

## SYNOPSIS
Allows adding new calendar events to calendar

## SYNTAX

```
New-CalendarEvent [[-Title] <String>] [[-Description] <String>] [[-StartDate] <DateTime>]
 [[-EndDate] <DateTime>] [[-Constraint] <String>] [[-Color] <String>] [[-BackgroundColor] <String>]
 [[-BorderColor] <String>] [[-TextColor] <String>] [[-Url] <String>] [-AllDayEvent] [<CommonParameters>]
```

## DESCRIPTION
Allows adding new calendar events to calendar

## EXAMPLES

### EXAMPLE 1
```
New-HTMLCalendar {
    New-CalendarEvent -Title 'Active Directory Meeting' -Description 'We will talk about stuff' -StartDate (Get-Date)
    # End date is required for the colors to work...
    New-CalendarEvent -Title 'Lunch' -StartDate (Get-Date).AddDays(2).AddHours(-3) -EndDate (Get-Date).AddDays(3) -Description 'Very long lunch' -TextColor DeepSkyBlue -BackgroundColor yellow -BorderColor Red
}
```

## PARAMETERS

### -Title
The text that will appear on an event.

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

### -Description
The text that will appear on an event when hovering over

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartDate
When your event begins.
If your event is explicitly allDay, hour, minutes, seconds and milliseconds will be ignored.

```yaml
Type: System.DateTime
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndDate
hen your event ends.
If your event is explicitly allDay, hour, minutes, seconds and milliseconds will be ignored.
If omitted, your events will appear to have the default duration.

```yaml
Type: System.Nullable`1[System.DateTime]
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Constraint
A groupId belonging to other events, "businessHours" or "availableForMeeting"

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Color
An alias for specifying the backgroundColor and borderColor at the same time.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
Sets backround color.
Only works if EndDate is provided.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderColor
Sets border color.
Only works if EndDate is provided.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TextColor
Sets color of Text.
Only works if EndDate is provided.

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

### -Url
A URL that will be visited when this event is clicked by the user.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Uri

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllDayEvent
Determines if the event is shown in the "all-day" section of the view, if applicable.
Determines if time text is displayed in the event.
If this value is not specified, it will be inferred by the start and end properties

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Keep in mind that colors like background, border, text work only if there's EndDate.
If there's no end date the color "color" is used only

## RELATED LINKS
