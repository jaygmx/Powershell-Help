---
external help file: UniversalDashboard-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDTreeView.md
schema: 2.0.0
---

# Remove-UDCookie

## SYNOPSIS
Outputs data as a table.

## SYNTAX

## DESCRIPTION
Outputs data as a table.

## EXAMPLES

### Example 1
```
PS C:\>  New-UDTable -Title "Process Ids" -Header @("Name", "Process Id") -Endpoint {
    Get-Process -Name Chrome | Out-UDTableData -Property @("name", "id")
}
```

Outputs data from Get-Process as a table.
Selects the Name and ID property from each item.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Object
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
