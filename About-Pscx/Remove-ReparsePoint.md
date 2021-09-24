---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Remove-ReparsePoint

## SYNOPSIS
PSCX Cmdlet: Removes NTFS reparse junctions and symbolic links.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Remove-ReparsePoint [-Path] <String[]> [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Remove-ReparsePoint [-LiteralPath] <String[]> [<CommonParameters>]
```

## DESCRIPTION
Removes NTFS reparse junctions and symbolic links.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -LiteralPath
@{Text=}

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Path to the new link.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS

[New-Hardlink]()

[New-Junction]()

[Get-MountPoint]()

[Remove-MountPoint]()

[Get-ReparsePoint]()

[New-Symlink]()

