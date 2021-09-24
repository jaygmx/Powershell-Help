---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDLink.md
schema: 2.0.0
---

# New-UDMuLink

## SYNOPSIS


## SYNTAX

### text
```
New-UDMuLink [-Id <String>] [-url <String>] [-underline <String>] [-style <Hashtable>] [-variant <String>]
 [-ClassName <String>] [-openInNewWindow] [-text <String>] [<CommonParameters>]
```

### content
```
New-UDMuLink [-Id <String>] [-url <String>] [-underline <String>] [-style <Hashtable>] [-ClassName <String>]
 [-openInNewWindow] [-content <ScriptBlock>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```
PS C:\> 
```



## PARAMETERS

### -ClassName
Set the Html class name

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

### -Id
Enter id for this object

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

### -content
The object or object to make as link

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: content
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
Type: System.Management.Automation.SwitchParameter
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
Type: System.Collections.Hashtable
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
Type: System.String
Parameter Sets: text
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
Type: System.String
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
Type: System.String
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
Type: System.String
Parameter Sets: text
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

## RELATED LINKS
