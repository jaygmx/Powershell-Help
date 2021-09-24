---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Set-VolumeLabel

## SYNOPSIS
PSCX Cmdlet: Modifies the label shown in Windows Explorer for a particular disk volume.

## SYNTAX

```
Set-VolumeLabel [[-Path] <String>] [[-Label] <String>] [<CommonParameters>]
```

## DESCRIPTION
Modifies the label shown in Windows Explorer for a particular disk volume.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Path
Path to the root directory of a file system volume.
This can be a folder where a volume is mounted.
If not specified, defaults to the root of the current FileSystem location.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Label
New volume label.
If not specified, the volume label will be blank.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS
