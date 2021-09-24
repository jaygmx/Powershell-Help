---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/tricks/assemblies/load-from-memory
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.5/Get-PSOneDirectory.ps1
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.5/Internal/Install-LongPathSupport.ps1
schema: 2.0.0
---

# Get-PSOneDirectory

## SYNOPSIS
Lists the content of a folder and supports long path names (\>256 characters)

## SYNTAX

```
Get-PSOneDirectory [-Path] <String> [<CommonParameters>]
```

## DESCRIPTION
Uses the Microsoft.Experimental.IO assembly to list folder contents without
path name length limitations.
You can use this function to search for and identify 
files and folders that use long path names.

## EXAMPLES

### EXAMPLE 1
```
Get-PSOneDirectory -Path C:\Windows -ErrorAction SilentlyContinue
Dumps the entire content of the windows folder and reports all files
and folders and their path length. Error messages due to folders
where you have no access permissions are suppressed.
```

### EXAMPLE 2
```
Get-PSOneDirectory -Path C:\Windows -ErrorAction SilentlyContinue |
  Where-Object PathLength -gt 200
Lists files and folders with a path length of greater than 200 characters. 
Error messages due to folders where you have no access permissions are suppressed.
```

## PARAMETERS

### -Path
Folder path to enumerate

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
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

[https://powershell.one/tricks/assemblies/load-from-memory
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.5/Get-PSOneDirectory.ps1
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.5/Internal/Install-LongPathSupport.ps1](https://powershell.one/tricks/assemblies/load-from-memory
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.5/Get-PSOneDirectory.ps1
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.5/Internal/Install-LongPathSupport.ps1)

[https://powershell.one/tricks/assemblies/load-from-memory
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.5/Get-PSOneDirectory.ps1
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.5/Internal/Install-LongPathSupport.ps1]()

