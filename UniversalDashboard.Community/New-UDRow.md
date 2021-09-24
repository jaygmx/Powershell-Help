---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDRow.md
schema: 2.0.0
---

# New-UDRow

## SYNOPSIS
Creates a new row on the dashboard.

## SYNTAX

### static (Default)
```
New-UDRow [-Id <String>] [[-Columns] <ScriptBlock>] [<CommonParameters>]
```

### dynamic
```
New-UDRow [-Id <String>] [-Endpoint <Object>] [-AutoRefresh] [-RefreshInterval <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Creates a new row on the dashboard.
Columns are defined with New-UDColumn.

## EXAMPLES

### Example 1
```
New-UDRow {
	New-UDColumn -Size 6 {
		New-UDCard -Content {} -BackgroundColor black
	}
	New-UDColumn -Size 6 {
		New-UDCard -Content {} -BackgroundColor black
	}
}
```

Defines a row with two columns are equal size.

### Example 2
```
New-UDRow {
	New-UDColumn -Size 6 {
		New-UDRow {
			New-UDColumn -Size 6 {
				New-UDCard -Content {} -BackgroundColor black
			}
			New-UDColumn -Size 6 {
				New-UDCard -Content {} -BackgroundColor black
			}
		}
	}
	New-UDColumn -Size 6 {
		New-UDCard -Content {} -BackgroundColor black
	}
}
```

Defines a row with two columns are equal size.
Inside the first column is another row with two columns.

## PARAMETERS

### -AutoRefresh
Whether this row should autorefresh.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: dynamic
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Columns
The columns to define for the row.
These columns should be defined using New-UDColumn.

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: static
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Endpoint
The endpoint to call when generating the content for this row.

```yaml
Type: System.Object
Parameter Sets: dynamic
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The ID of the row.
This is the HTML markup ID.

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

### -RefreshInterval
The number of seconds between refreshes.

```yaml
Type: System.Int32
Parameter Sets: dynamic
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
