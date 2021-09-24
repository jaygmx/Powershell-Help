---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# New-Hardlink

## SYNOPSIS
PSCX Cmdlet: Creates filesystem hard links.
The hardlink and the target must reside on the same NTFS volume.

## SYNTAX

```
New-Hardlink [-LiteralPath] <PscxPathInfo> [-TargetPath] <PscxPathInfo> [-WhatIf] [-Confirm]
 [<CommonParameters>]
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
Type: Pscx.IO.PscxPathInfo
Parameter Sets: (All)
Aliases: Path

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TargetPath
@{Text=}

```yaml
Type: Pscx.IO.PscxPathInfo
Parameter Sets: (All)
Aliases: Target, PSPath

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

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

[New-Junction]()

[Get-MountPoint]()

[Remove-MountPoint]()

[Get-ReparsePoint]()

[Remove-ReparsePoint]()

[New-Symlink]()

