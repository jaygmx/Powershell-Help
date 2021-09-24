---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-PscxClipboard

## SYNOPSIS
PSCX Cmdlet: Gets data from the clipboard.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-PscxClipboard [-Text] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-PscxClipboard [-FragmentOnly] [-Html] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Get-PscxClipboard [-Rtf] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_4
```
Get-PscxClipboard [-Csv] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_5
```
Get-PscxClipboard [-Image] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_6
```
Get-PscxClipboard [-Files] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_7
```
Get-PscxClipboard [-Audio] [<CommonParameters>]
```

## DESCRIPTION
Gets data from the clipboard.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Audio
Retrieves audio data from clipboard.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_7
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Csv
Retrieves CSV data from clipboard.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Files
Retrieves list of file names from clipboard.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_6
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FragmentOnly
Retrieves only the selected fragment of the HTML data.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Html
Retrieves HTML data from clipboard.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Image
Retrieves image data from clipboard.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_5
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Rtf
Retrieves rich text data from clipboard.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text
Retrieves plain text data from clipboard.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
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

## OUTPUTS

## NOTES
*

## RELATED LINKS

[Out-PscxClipboard]()

[Set-PscxClipboard]()

[Write-PscxClipboard]()

