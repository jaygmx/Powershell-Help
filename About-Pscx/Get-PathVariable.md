---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-PathVariable

## SYNOPSIS
PSCX Cmdlet: Gets the specified path-oriented environment variable.

## SYNTAX

```
Get-PathVariable [[-Name] <String>] [-RemoveEmptyPaths] [-StripQuotes] [-Target <EnvironmentVariableTarget>]
 [<CommonParameters>]
```

## DESCRIPTION
Gets the specified path-oriented environment variable and outputs an array of strings. 
One string for each path. 
The environment variable string is split a semi-colon and you can option specify that empty paths be removed and unnecessary quotes be removed from each path.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
Get-PathVariable Path
```

Gets the Path environment variable from the Process scope as an array of strings.

### EXAMPLE 2
PS C:\\\>

```
Get-PathVariable Path -Target User
```

Gets the Path environment variable as it is configured in the User scope.

### EXAMPLE 3
PS C:\\\>

```
Get-PathVariable Path -RemoveEmptyPaths -StripQuotes -Target Machine | Set-PathVariable Path -Target Machine
```

Gets the Machine scope Path environment variable while removing unnecessary quotes and empty paths and then sets it to the updated value.
This enviornment variable will be persisted across PowerShell sessions.

## PARAMETERS

### -Name
The name of the environment variable to get. 
Typically either Path, Lib, Include, etc.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveEmptyPaths
Empty paths, as represented by back-to-back semi-colons will be removed from the output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -StripQuotes
Removes unnecessary quotes from each path.
Most path-oriented environments variables do not require quotes around paths (even those paths with spaces in them). 
Since the semi-colon is not a valid path character it is sufficient to mark the beginning and ending of a path.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Target
Specifies which target scope to get: Process (default), User or Machine.

```yaml
Type: EnvironmentVariableTarget
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

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-PathVariable]()

[Set-PathVariable]()

[Pop-EnvironmentBlock]()

[Push-EnvironmentBlock]()

