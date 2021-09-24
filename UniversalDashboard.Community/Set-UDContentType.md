---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDTreeView.md
schema: 2.0.0
---

# Set-UDContentType

## SYNOPSIS
Sets the content-type HTTP header for a HTTP response.

## SYNTAX

```
Set-UDContentType [-ContentType] <Object> [<CommonParameters>]
```

## DESCRIPTION
Sets the content-type HTTP header for a HTTP response.
This should be in control's Endpoint script blocks.

## EXAMPLES

### Example 1
```
PS C:\> Set-UDContentType -ContentType "application/xml"
```

Sets the content type to XML if an endpoint wanted to return XML.

## PARAMETERS

### -ContentType
The content type to set.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
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
