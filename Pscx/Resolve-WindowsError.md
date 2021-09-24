---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# Resolve-WindowsError

## SYNOPSIS
Resolves a Windows error number a textual description of the error.

## SYNTAX

```
Resolve-WindowsError [-ErrorNumber] <Int32[]> [<CommonParameters>]
```

## DESCRIPTION
Resolves a Windows error number a textual description of the error.
The Windows
error number is typically retrieved via the Win32 API GetLastError() but it is
typically displayed in messages to the end user.

## EXAMPLES

### EXAMPLE 1
```
Resolve-WindowsError 5
Access is denied
```

## PARAMETERS

### -ErrorNumber
The Windows error code number to resolve.

```yaml
Type: System.Int32[]
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
Aliases:  rvwer

## RELATED LINKS
