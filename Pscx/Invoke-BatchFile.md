---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Invoke-BatchFile

## SYNOPSIS
Invokes the specified batch file and retains any environment variable changes it makes.

## SYNTAX

```
Invoke-BatchFile [[-Path] <String>] [[-Parameters] <String>]
```

## DESCRIPTION
Invoke the specified batch file (and parameters), but also propagate any
environment variable changes back to the PowerShell environment that
called it.

## EXAMPLES

### EXAMPLE 1
```
Invoke-BatchFile "$env:ProgramFiles\Microsoft Visual Studio 9.0\VC\vcvarsall.bat"
Invokes the vcvarsall.bat file.  All environment variable changes it makes will be
propagated to the current PowerShell session.
```

## PARAMETERS

### -Path
Path to a .bat or .cmd file.

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

### -Parameters
Parameters to pass to the batch file.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
Author: Lee Holmes

## RELATED LINKS
