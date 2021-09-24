---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Format-Byte

## SYNOPSIS
PSCX Cmdlet: Displays numbers in multiples of byte units.

## SYNTAX

```
Format-Byte [-Value] <Int64> [<CommonParameters>]
```

## DESCRIPTION
Turns numbers into nicely formatted byte count, using the highest possible unit.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
10560 | Format-Byte
```

Returns "10,313 KB".

## PARAMETERS

### -Value
The byte count to be formated.

```yaml
Type: Int64
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
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
