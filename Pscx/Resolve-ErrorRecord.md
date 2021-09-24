---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# Resolve-ErrorRecord

## SYNOPSIS
Resolves the PowerShell error code to a textual description of the error.

## SYNTAX

```
Resolve-ErrorRecord [[-ErrorRecord] <ErrorRecord[]>] [<CommonParameters>]
```

## DESCRIPTION
Use when reporting an error or ask a question about a exception you
are seeing. 
This function provides all the information we have
about the error message making it easier to diagnose what is
actually going on.

## EXAMPLES

### EXAMPLE 1
```
Resolve-ErrorRecord
Resolves the most recent PowerShell error code to a textual description of the error.
```

## PARAMETERS

### -ErrorRecord
The ErrorRecord to resolve into a useful error report.
The default value
is $Error\[0\] - the last error that occurred.

```yaml
Type: System.Management.Automation.ErrorRecord[]
Parameter Sets: (All)
Aliases:

Required: False
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
Aliases:  rver

## RELATED LINKS
