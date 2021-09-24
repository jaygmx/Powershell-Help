---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Set-PscxClipboard

## SYNOPSIS
PSCX Cmdlet: Puts the specified object into the system clipboard.

## SYNTAX

### Text (Default)
```
Set-PscxClipboard [-Text <String>] [<CommonParameters>]
```

### Image
```
Set-PscxClipboard [-Image <Image>] [<CommonParameters>]
```

### Files
```
Set-PscxClipboard [-Files <FileSystemInfo[]>] [<CommonParameters>]
```

### Html
```
Set-PscxClipboard [-Html <String>] [<CommonParameters>]
```

### Rtf
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
Type: System.IO.FileSystemInfo[]
Parameter Sets: Files
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
Type: System.String
Parameter Sets: Html
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
Type: System.Drawing.Image
Parameter Sets: Image
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
Type: System.String
Parameter Sets: Rtf
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
Type: System.String
Parameter Sets: Text
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

## RELATED LINKS

[Get-PscxClipboard]()

[Out-PscxClipboard]()

[Write-PscxClipboard]()

