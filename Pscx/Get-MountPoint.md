---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-MountPoint

## SYNOPSIS
PSCX Cmdlet: Returns all mount points defined for a specific root path.

## SYNTAX

```
Get-MountPoint [[-Volume] <String>] [<CommonParameters>]
```

## DESCRIPTION
Returns all mount points defined for a specific root path.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Volume
When specified, gets mount points on the specified volume; otherwise, returns mount points on all volumes.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
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

[New-Hardlink]()

[New-Junction]()

[Remove-MountPoint]()

[Get-ReparsePoint]()

[Remove-ReparsePoint]()

[New-Symlink]()

