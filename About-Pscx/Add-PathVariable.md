---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Add-PathVariable

## SYNOPSIS
PSCX Cmdlet: Adds the specified paths to the end of the named, path-oriented environment variable.

## SYNTAX

```
Add-PathVariable [-Value] <String[]> [-Name <String>] [-Prepend] [-Target <EnvironmentVariableTarget>]
 [<CommonParameters>]
```

## DESCRIPTION
Adds the specified paths to the end of the named, path-oriented environment variable by taking the paths specified by the Value parameter and concatenating them into a semi-colon separated string. 
The paths can be prepended to the environment variable by using the -Prepend switch parameter.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
Add-PathVariable Lib C:\Lib, C:\ProjA\Lib
```

Adds the specified paths to the end of current Lib environment variable setting (creating it if necessary) in the Process scope.

### EXAMPLE 2
PS C:\\\>

```
Add-PathVariable Lib C:\Lib, C:\ProjA\Lib -Target User
```

Adds the specified paths to the end of current Lib environment variable setting (creating it if necessary) in the User scope.

## PARAMETERS

### -Value
The paths to concat together with semi-colon separators.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
The name of the environment variable to add to. 
Typically either Path (default), Lib, Include, etc.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Path
Accept pipeline input: False
Accept wildcard characters: False
```

### -Prepend
The specified paths will be prepended to the environment variable instead of appended.

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
Specifies which target scope to modify. 
The valid values are Process (default), User or Machine. 
Using either the User or the Machine target scope will cause the new value to persist.

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

[Get-PathVariable]()

[Set-PathVariable]()

[Pop-EnvironmentBlock]()

[Push-EnvironmentBlock]()

