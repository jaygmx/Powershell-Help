---
external help file: Microsoft.PowerShell.PSReadLine2.dll-help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-PSReadLineKeyHandler

## SYNOPSIS
Gets the key bindings for the PSReadLine module.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-PSReadLineKeyHandler [-Bound] [-Unbound] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-PSReadLineKeyHandler [-Chord] <String[]> [<CommonParameters>]
```

## DESCRIPTION
Gets the key bindings for the PSReadLine module.

If no parameter is specified, returns all bound keys functions.

If '-Bound' is specified and '-Unbound' is not specified, only bound keys are returned.

If '-Unbound' is specified and '-Bound' is not specified, only unbound keys are returned.

If both '-Bound' and '-Unbound' are specified, returns all bound keys and unbound functions.

If '-Chord' is specified, returns the specific bound keys.

## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Bound
Include functions that are bound.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
```

### -Unbound
Include functions that are unbound.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Chord
Return only functions bound to specific keys or sequences.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: Key

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
You cannot pipe objects to Get-PSReadLineKeyHandler

## OUTPUTS

### Microsoft.PowerShell.KeyHandler
Returns one entry for each key binding (or chord) for bound functions and/or one entry for each unbound function

## NOTES
*

## RELATED LINKS

[about_PSReadLine]()

