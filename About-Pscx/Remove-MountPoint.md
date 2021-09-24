---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Remove-MountPoint

## SYNOPSIS
PSCX Cmdlet: Removes a mount point, dismounting the current media if any.
If used against the root of a fixed drive, removes the drive letter assignment.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Remove-MountPoint [-Path] <String[]> [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Remove-MountPoint [-LiteralPath] <String[]> [<CommonParameters>]
```

## DESCRIPTION
Removes a mount point, dismounting the current media if any.
If used against the root of a fixed drive, removes the drive letter assignment.

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
@{Text=}

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

[Get-ReparsePoint]()

[Remove-ReparsePoint]()

[New-Symlink]()

