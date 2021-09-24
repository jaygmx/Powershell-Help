---
external help file: PSScriptTools-help.xml
Module Name: PSScriptTools
online version: https://bit.ly/33UwYKo
schema: 2.0.0
---

# Get-PathVariable

## SYNOPSIS
Get information from locations in %PATH%.

PSCX Cmdlet: Gets the specified path-oriented environment variable.

## SYNTAX

```
Get-PathVariable [[-Scope] <String>] [<CommonParameters>]
```

## DESCRIPTION
Use this command to test the locations specified in the %PATH% environment variable.
On Windows platforms, you can distinguish between settings set per machine and those set per user.
On non-Windows platforms, the scope will be Process.

Gets the specified path-oriented environment variable and outputs an array of strings. 
One string for each path. 
The environment variable string is split a semi-colon and you can option specify that empty paths be removed and unnecessary quotes be removed from each path.

## EXAMPLES

### Example 1
```
PS C:\> Get-PathVariable

Scope   UserName Path                                            Exists
-----   -------- ----                                            ------
User    Jeff     C:\Program Files\kdiff3                         True
User    Jeff     C:\Program Files (x86)\Bitvise SSH Client       True
User    Jeff     C:\Program Files\OpenSSH                        True
...
Machine Jeff     C:\WINDOWS                                      True
Machine Jeff     C:\WINDOWS\system32                             True
Machine Jeff     C:\WINDOWS\System32\Wbem                        True
...
```

### Example 2
```
PS /home/jeff> Get-PathVariable | Where-Object {-Not $_.exists}

Scope        : Process
Computername : Bovine320
UserName     : jeff
Path         : /snap/bin
Exists       : False
```

This example is on a Linux platform, finding locations that don't exist or can be verified.
You could run the same command on Windows.

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

### -Scope
On Windows platforms you can distinguish between Machine and User specific settings.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: All, User, Machine

Required: False
Position: 0
Default value: All
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### EnvPath
## NOTES
Learn more about PowerShell: http://jdhitsolutions.com/blog/essential-powershell-resources/

## RELATED LINKS

[Add-PathVariable]()

[Set-PathVariable]()

[Pop-EnvironmentBlock]()

[Push-EnvironmentBlock]()

