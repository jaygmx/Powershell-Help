---
external help file: UniversalDashboard.dll-Help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDInput.md
schema: 2.0.0
---

# New-UDInputField

## SYNOPSIS
Creates input fields for New-UDInput.

## SYNTAX

```
New-UDInputField -Name <String> [-Values <Object[]>] [-DefaultValue <Object>] [-Placeholder <String[]>]
 [-Disabled] [-Type <String>] [-OkText <String>] [-CancelText <String>] [-ClearText <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Creates input fields for New-UDInput.
This cmdlet should be used within New-UDInput's -Content parameter.

## EXAMPLES

### Example 1
```
PS C:\> New-UDInput -Content {
    New-UDInputField -Type textbox -Name UserName 
} -Endpoint {
    param($UserName)
}
```

Creates a new input field within an input to accept text input.

### Example 2
```
PS C:\> New-UDInput -Content {
    New-UDInputField -Type select -Name language -Values @("PowerShell", "Python", "C#")
} -Endpoint {
    param($language)
}
```

Creates a new input field within an input to accept a selection of values in a select box.

## PARAMETERS

### -CancelText
Cancel text for the datetime selector.

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

### -ClearText
Clear text for the datetime selector.

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

### -DefaultValue
The default value for this field.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The name of this field.
This is also the variable name passed into the Endpoint block in New-UDInput.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OkText
Ok text for the datetime selector.

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

### -Placeholder
Place holders to use as display text.
Use an array for select fields and a single item for text fields.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
The type of field.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: textbox, checkbox, select, radioButtons, password, textarea, switch, date, file, time, binaryFile

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Values
Valid values for this field.
Only applies to select and radio buttons.

```yaml
Type: System.Object[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Disabled
{{ Fill Disabled Description }}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
