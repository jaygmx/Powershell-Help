---
external help file: TSUtils-help.xml
Module Name: TSUtils
online version:
schema: 2.0.0
---

# New-ModuleTemplate

## SYNOPSIS
Generate module scaffolding and boilerplate.

## SYNTAX

```
New-ModuleTemplate [-Names] <String[]> [[-Path] <FileInfo>] [[-Author] <String>] [[-CompanyName] <String>]
 [[-Description] <String>] [[-RequiredModules] <String[]>] [-UncommentConfig] [<CommonParameters>]
```

## DESCRIPTION
Creates the following:

- Public, Private & Classes directories for storing module functions.

- A psm1 script that dot sources functions from Public & Private, but exports
  only those in Public.

- A manifest file.

- Two scripts in the root of the module that are dot sourced in the .psm1
  file.
One defines color splatting hash tables, the other provides support
  for storing sensitive data in variables in a Config.psd1 file that is
  ignored by git.

## EXAMPLES

### EXAMPLE 1
```
$Params = @{
Name = Module1,Module2,Module3
Path = "C:\MyModules"
Author = "Me Myself & I"
CompanyName = "My Awesome Company"
Description = "This module will rock your world!"
RequiredModules = 'All','My','Other','Modules'
}
New-ModuleTemplate @Params
```

## PARAMETERS

### -Names
The names of the modules you want to create.

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

### -Path
The path to store these modules in.
Defaults to the last path found in
$env:PSModulePath.

```yaml
Type: System.IO.FileInfo
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: ($env:PSModulePath -split ':|;' | Select-Object -last 1)
Accept pipeline input: False
Accept wildcard characters: False
```

### -Author
Name of the modules author.
This will be inserted into the Author and
Copyright fields in the manifest file.
Defaults to the current users' name.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: $env:USER
Accept pipeline input: False
Accept wildcard characters: False
```

### -CompanyName
This will be inserted into the Company field of the manifest file.
Defaults
to nil.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Description of the module.
This will be inserted into the description field
of the module manifest and at the top of the main README.md.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: Module Description
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequiredModules
List of modules that this module depends on.
Will be inserted into the
RequiredModules field of the manifest file.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -UncommentConfig
A switch that uncomments a line in the psm1 file that dot sources the
configuration management script.
This is stored in Config.ps1 and allows
reading in of sensitive data stored in a Config.psd1 for setting variables
available in the modules' scope.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
