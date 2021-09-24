---
external help file: ZLocation-help.xml
Module Name: ZLocation
online version: https://github.com/vors/ZLocation
schema: 2.0.0
---

# Invoke-ZLocation

## SYNOPSIS
Jump to popular directories.

## SYNTAX

```
Invoke-ZLocation [[-match] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
This is the main entry point in the interactive usage of ZLocation.
It's intended to be used as an alias z.

Usage:
    z - prints available directories
    z -l foo - prints available directories scoped to foo query
    z foo - jumps into the location that matches foo
    z foo \<TAB\> - pressing tab cycles through different matches for foo
    z - - undos the last z jump.

## EXAMPLES

### EXAMPLE 1
```
z
Weight Path
------ ----
    7 C:\Windows
    1 C:\Windows\System
    27 C:\WINDOWS\system32
    [...]
```

### EXAMPLE 2
```
z foo
C:\foo>
```

### EXAMPLE 3
```
z foo <PRESS TAB; NOT ENTER>
C:\>z C:\foo <PRESS TAB AGAIN>
C:\>z C:\another_less_popular\foo <PRESS TAB AGAIN>
C:\>z C:\least_popular\foo
C:\least_popular\foo>
```

### EXAMPLE 4
```
z -l sys
Weight Path
------ ----
    27 C:\WINDOWS\system32
     1 C:\Windows\System
```

### EXAMPLE 5
```
z foo
C:\foo>z bar
C:\baz\bar> z -
C:\foo>z -
C:\>z -
C:\>#no-op
```

## PARAMETERS

### -match
{{ Fill match Description }}

```yaml
Type: System.String[]
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

[https://github.com/vors/ZLocation](https://github.com/vors/ZLocation)

