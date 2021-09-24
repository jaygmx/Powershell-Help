---
external help file: AdminToolbox.Exchange-help.xml
Module Name: AdminToolbox.Exchange
online version:
schema: 2.0.0
---

# Get-MailLog

## SYNOPSIS

## SYNTAX

```
Get-MailLog [-Start] <Object> [-End] <Object> [-ExportPath] <Object> [-ResultSize] <Object> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Creates a csv file containing logs of mail in a given time frame.

## EXAMPLES

### EXAMPLE 1
```
Specify the date range, report path, and amount of records to return.
```

Get-MailLog -Start 05/14/2017 -End 05/14/2018 -ExportPath C:\MailLog.CSV -Resultsize 10000

## PARAMETERS

### -Start
Start date for the search

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -End
End date for the search

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportPath
Path for the csv to be saved to

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResultSize
Maximum number of results returned

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 4
Default value: None
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
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Requires the Microsoft Exchange module.

## RELATED LINKS

[Get-MessageTrackingLog]()

