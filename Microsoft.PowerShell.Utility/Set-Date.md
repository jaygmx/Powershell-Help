---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
Module Name: Microsoft.PowerShell.Utility
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/set-date?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Set-Date

## SYNOPSIS
Changes the system time on the computer to a time that you specify.

## SYNTAX

### Date (Default)
```
Set-Date [-Date] <DateTime> [-DisplayHint <DisplayHintType>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Adjust
```
Set-Date [-Adjust] <TimeSpan> [-DisplayHint <DisplayHintType>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The \`Set-Date\` cmdlet changes the system date and time on the computer to a date and time that you specify.
You can specify a new date and/or time by typing a string or by passing a DateTime or TimeSpan object to \`Set-Date\`.
To specify a new date or time, use the Date parameter.
To specify a change interval, use the Adjust parameter.

## EXAMPLES

### Example 1: Add three days to the system date
```
Set-Date -Date (Get-Date).AddDays(3)
```

### Example 2: Set the system clock back 10 minutes
```
Set-Date -Adjust -0:10:0 -DisplayHint Time
```

### Example 3: Set the date and time to a variable value
```
$T = Get-Date
Set-Date -Date $T
```

### Example 4: Add 90 minutes to the system clock
```
$90mins = New-TimeSpan -Minutes 90
Set-Date -Adjust $90mins
```

## PARAMETERS

### -Adjust
Specifies the value for which this cmdlet adds or subtracts from the current date and time.
can type an adjustment in standard date and time format for your locale or use the Adjust parameter to pass a TimeSpan object from \`New-TimeSpan\` to \`Set-Date\`.

```yaml
Type: System.TimeSpan
Parameter Sets: Adjust
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Date
Changes the date and time to the specified values.
You can type a new date in the short date format and a time in the standard time format for your locale.
Or, you can pass a DateTime object from \`Get-Date\`.

If you specify a date, but not a time, \`Set-Date\` changes the time to midnight on the specified date.
If you specify only a time, it does not change the date.

```yaml
Type: System.DateTime
Parameter Sets: Date
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -DisplayHint
Specifies which elements of the date and time are displayed.The acceptable values for this parameter are:

- Date - displays only the date. - Time - displays only the time. - DateTime - displays the date and time.

This parameter affects only the display.
It does not affect the DateTime object that \`Get-Date\` retrieves.

```yaml
Type: Microsoft.PowerShell.Commands.DisplayHintType
Parameter Sets: (All)
Aliases:
Accepted values: Date, Time, DateTime

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.DateTime
You can pipe a date to \`Set-Date\`.

## OUTPUTS

### System.DateTime
\`Set-Date\` returns an object that represents the date that it set.

## NOTES
- Use this cmdlet cautiously when changing the date and time on the computer. The change might   prevent the computer from receiving system-wide events and updates that are triggered by a date or   time. Use the WhatIf and Confirm parameters to avoid errors. - You can use standard .NET methods with the DateTime and TimeSpan objects used with   \`Set-Date\`, such as AddDays , AddMonths , and FromFileTime . For more information, see DateTime Methods (/dotnet/api/system.datetime)and TimeSpan Methods (/dotnet/api/system.timespan)in the .NET SDK.

## RELATED LINKS

[Get-Date]()

[New-TimeSpan]()

