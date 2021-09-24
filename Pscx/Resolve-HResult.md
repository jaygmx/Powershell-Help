---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# Resolve-HResult

## SYNOPSIS
Resolves the hresult error code to a textual description of the error.

## SYNTAX

```
Resolve-HResult [-HResult] <Int64[]> [<CommonParameters>]
```

## DESCRIPTION
Resolves the hresult error code to a textual description of the error.

## EXAMPLES

### EXAMPLE 1
```
Resolve-HResult -2147023293
Fatal error during installation. (Exception from HRESULT: 0x80070643)
```

## PARAMETERS

### -HResult
The hresult error code to resolve.

```yaml
Type: System.Int64[]
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
Aliases:  rvhr

## RELATED LINKS
