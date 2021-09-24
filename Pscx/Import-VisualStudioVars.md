---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Import-VisualStudioVars

## SYNOPSIS
Imports environment variables for the specified version of Visual Studio.

## SYNTAX

```
Import-VisualStudioVars [[-VisualStudioVersion] <String>] [[-Architecture] <String>]
 [-RequireWorkload <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Imports environment variables for the specified version of Visual Studio.
This function requires the PowerShell Community Extensions.
To find out
the most recent set of Visual Studio environment variables imported use
the cmdlet Get-EnvironmentBlock. 
If you want to revert back to a previous
Visul Studio environment variable configuration use the cmdlet
Pop-EnvironmentBlock.

## EXAMPLES

### EXAMPLE 1
```
Import-VisualStudioVars 2015
```

Sets up the environment variables to use the VS 2015 tools.
If 
VsDevCmd.bat is found then it will use that.
Otherwise, vcvarsall.bat will
be used with an architecture of either x86 for 32-bit Powershell, or amd64
for 64-bit Powershell.

### EXAMPLE 2
```
Import-VisualStudioVars 2013 arm
```

Sets up the environment variables for the VS 2013 ARM tools.

### EXAMPLE 3
```
Import-VisualStudioVars 2017 -Architecture amd64 -RequireWorkload Microsoft.VisualStudio.Component.VC.Tools.x86.x64
```

Finds an instance of VS 2017 that has the required workload and sets up
the environment variables to use that instance of the VS 2017 tools. 
To see a full list of available workloads, execute:
Get-VSSetupInstance | Foreach-Object Packages | Foreach-Object Id | Sort-Object

## PARAMETERS

### -VisualStudioVersion
The version of Visual Studio to import environment variables for.
Valid
values are 2008, 2010, 2012, 2013, 2015, 2017 and 2019.

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

### -Architecture
Selects the desired architecture to configure the environment for.
If this parameter isn't specified, the command will attempt to locate and
use VsDevCmd.bat. 
If VsDevCmd.bat can't be found (not installed) then the
command will use vcvarsall.bat with either the argument x86 if running in
32-bit PowerShell or amd64 if running in 64-bit PowerShell.
Other valid
values are: arm, x86_arm, x86_amd64, amd64_x86.

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

### -RequireWorkload
This parameter applies to Visual Studio 2017 and higher. 
It allows you 
to specify which workloads are required for the environment you desire to
import. 
This can be used when you have multiple versions of Visual Studio
2017 installed and different versions support different workloads e.g.
perhaps only the "Preview" version supports the 
Microsoft.VisualStudio.Component.VC.Tools.x86.x64 workload.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
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
