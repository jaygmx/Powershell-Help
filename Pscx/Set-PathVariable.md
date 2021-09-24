---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Set-PathVariable

## SYNOPSIS
PSCX Cmdlet: Sets the specified path-oriented environment variable.

## SYNTAX

```
Set-PathVariable [-Value] <String[]> [-Name <String>] [-Target <EnvironmentVariableTarget>]
 [<CommonParameters>]
```

## DESCRIPTION
Sets the specified path-oriented environment variable by taking the paths specified by the Value parameter and concatenating them into a semi-colon separated string.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
Set-PathVariable Lib C:\Lib, C:\ProjA\Lib
```

Sets the Lib environment variable (creating it if necessary) to the value "C:\Lib;C:\ProjA\Lib" in the Process scope.

### EXAMPLE 2
PS C:\\\>

```
Set-PathVariable Lib C:\Lib, C:\ProjA\Lib -Target User
```

Sets the Lib environment variable (creating it if necessary) to the value "C:\Lib;C:\ProjA\Lib" in the User scope. 
This enviornment variable will be persisted across PowerShell sessions.

### EXAMPLE 3
PS C:\\\>

```
Get-PathVariable Path -RemoveEmptyPaths -StripQuotes -Target Machine | Set-PathVariable Path -Target Machine
```

Gets the Machine scope Path environment variable while removing unnecessary quotes and empty paths and then sets it to the updated value.
This enviornment variable will be persisted across PowerShell sessions.

## PARAMETERS

### -Value
The paths to concat together with semi-colon separators.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
The name of the environment variable to set. 
Typically either Path (default), Lib, Include, etc.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Path
Accept pipeline input: False
Accept wildcard characters: False
```

### -Target
Specifies which target scope to modify. 
The valid values are Process (default), User or Machine. 
Using either the User or the Machine target scope will cause the new value to persist.

```yaml
Type: System.EnvironmentVariableTarget
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Process
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS

[Add-PathVariable]()

[Get-PathVariable]()

[Pop-EnvironmentBlock]()

[Push-EnvironmentBlock]()

