---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDMonitor.md
schema: 2.0.0
---

# New-UDParagraph

## SYNOPSIS
Creates a new paragraph block.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDParagraph [-Color <DashboardColor>] [-Content <ScriptBlock>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDParagraph [-Color <DashboardColor>] [-Text <String>] [<CommonParameters>]
```

## DESCRIPTION
Creates a new paragraph block.

## EXAMPLES

### Example 1
```
PS C:\> New-UDParagraph -Content {
    "This is a paragraph of text"
}
```

Creates a new paragraph of text.

## PARAMETERS

### -Color
Text color for this paragraph.

```yaml
Type: DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Content
The content for this paragraph.

```yaml
Type: ScriptBlock
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text
Text for this paragraph.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
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
*

## RELATED LINKS
