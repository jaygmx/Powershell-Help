---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Set-PscxClipboard

## SYNOPSIS
PSCX Cmdlet: Puts the specified object into the system clipboard.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Set-PscxClipboard [-Image <Image>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Set-PscxClipboard [-Files <FileSystemInfo[]>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Set-PscxClipboard [-Text <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_4
```
Set-PscxClipboard [-Html <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_5
```
Set-PscxClipboard [-Rtf <String>] [<CommonParameters>]
```

## DESCRIPTION
Puts the specified object into the system clipboard.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Files
@{Text=}

```yaml
Type: FileSystemInfo[]
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Html
@{Text=}

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Image
@{Text=}

```yaml
Type: Image
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Rtf
@{Text=}

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_5
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Text
@{Text=}

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS

[Get-PscxClipboard]()

[Out-PscxClipboard]()

[Write-PscxClipboard]()

