---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-PscxClipboard

## SYNOPSIS
PSCX Cmdlet: Gets data from the clipboard.

## SYNTAX

### Text (Default)
```
Get-PscxClipboard [-Text] [<CommonParameters>]
```

### Html
```
Get-PscxClipboard [-Html] [-FragmentOnly] [<CommonParameters>]
```

### Rtf
```
Get-PscxClipboard [-Rtf] [<CommonParameters>]
```

### Csv
```
Get-PscxClipboard [-Csv] [<CommonParameters>]
```

### Image
```
Get-PscxClipboard [-Image] [<CommonParameters>]
```

### Files
```
Get-PscxClipboard [-Files] [<CommonParameters>]
```

### Audio
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Audio
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Csv
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Files
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Html
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Html
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Image
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Rtf
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Text
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

## RELATED LINKS

[Out-PscxClipboard]()

[Set-PscxClipboard]()

[Write-PscxClipboard]()

