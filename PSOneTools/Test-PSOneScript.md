---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/powershell-internals/parsing-and-tokenization/simple-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Test-PSOneScript.ps1
schema: 2.0.0
---

# Test-PSOneScript

## SYNOPSIS
Parses a PowerShell Script (*.ps1, *.psm1, *.psd1)

## SYNTAX

### Path (Default)
```
Test-PSOneScript -Path <String> [<CommonParameters>]
```

### Code
```
Test-PSOneScript -Code <String> [<CommonParameters>]
```

## DESCRIPTION
Invokes the simple PSParser and returns tokens and syntax errors

## EXAMPLES

### EXAMPLE 1
```
Test-PSOneScript -Path c:\test.ps1
Parses the content of c:\test.ps1 and returns tokens and syntax errors
```

### EXAMPLE 2
```
Get-ChildItem -Path $home -Recurse -Include *.ps1,*.psm1,*.psd1 -File |
   Test-PSOneScript |
   Out-GridView
```

parses all PowerShell files found anywhere in your user profile

### EXAMPLE 3
```
Get-ChildItem -Path $home -Recurse -Include *.ps1,*.psm1,*.psd1 -File |
   Test-PSOneScript |
   Where-Object Errors
```

parses all PowerShell files found anywhere in your user profile
and returns only those files that contain syntax errors

## PARAMETERS

### -Path
Path to PowerShell script file
can be a string or any object that has a "Path" 
or "FullName" property:

```yaml
Type: System.String
Parameter Sets: Path
Aliases: FullName

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Code
PowerShell Code as String
you can also submit a ScriptBlock which will automatically be converted
to a string.
ScriptBlocks by default cannot contain syntax errors because
they are parsed already.

```yaml
Type: System.String
Parameter Sets: Code
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one/powershell-internals/parsing-and-tokenization/simple-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Test-PSOneScript.ps1](https://powershell.one/powershell-internals/parsing-and-tokenization/simple-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Test-PSOneScript.ps1)

[https://powershell.one/powershell-internals/parsing-and-tokenization/simple-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Test-PSOneScript.ps1]()

