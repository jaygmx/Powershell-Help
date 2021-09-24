---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDMonitor.md
schema: 2.0.0
---

# New-UDMuLink

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDMuLink [-ClassName <String>] [-Id <String>] [-content <ScriptBlock>] [-openInNewWindow]
 [-style <Hashtable>] [-underline <String>] [-url <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDMuLink [-ClassName <String>] [-Id <String>] [-openInNewWindow] [-style <Hashtable>] [-text <String>]
 [-underline <String>] [-url <String>] [-variant <String>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -ClassName
Set the Html class name

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Enter id for this object

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -content
The object or object to make as link

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

### -openInNewWindow
Open the result in new window or in the current window

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -style
The css propertis for this object

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -text
The text to show as link

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

### -underline
Show line under the text or content

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Accepted values: none, hover, always

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -url
Enter url, this can be remote or local

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -variant
The pre configure style

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:
Accepted values: h1, h2, h3, h4, h5, h6, subtitle1, subtitle2, body1, body2, caption, button, overline, srOnly, inherit

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
