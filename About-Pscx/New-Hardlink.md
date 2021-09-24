---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# New-Hardlink

## SYNOPSIS
PSCX Cmdlet: Creates filesystem hard links.
The hardlink and the target must reside on the same NTFS volume.

## SYNTAX

```
New-Hardlink [-LiteralPath] <String> [-TargetPath] <String> [<CommonParameters>]
```

## DESCRIPTION
Creates filesystem hard links.
The hardlink and the target must reside on the same NTFS volume.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -LiteralPath
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TargetPath
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
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

[New-Junction]()

[Get-MountPoint]()

[Remove-MountPoint]()

[Get-ReparsePoint]()

[Remove-ReparsePoint]()

[New-Symlink]()

