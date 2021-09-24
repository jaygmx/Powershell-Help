---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDTreeView.md
schema: 2.0.0
---

# Out-UDGridData

## SYNOPSIS
Outputs data in a format that the jQuery DataTables grid will support.

## SYNTAX

```
Out-UDGridData [[-Data] <Object>] [[-TotalItems] <Int32>] [[-Depth] <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Outputs data in a format that the jQuery DataTables grid will support.

## EXAMPLES

### Example 1
```
PS C:\> New-UDGrid -Title "Process Information" -Headers @("Name", "Process Id", "Start Time", "Responding") -Properties @("Name", "Id", "StartTime", "Responding")  -Endpoint {
    Get-Process -Name Chrome | Out-UDGridData
}
```

Outputs the data from Get-Process to a New-UDGrid

## PARAMETERS

### -Data
The data to output.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Depth
The maximum object depth to serialize.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TotalItems
@{Text=}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Object
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
