---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-Parameter

## SYNOPSIS
Enumerates the parameters of one or more commands.

## SYNTAX

### ParameterName (Default)
```
Get-Parameter [-CommandName] <String[]> [-ModuleName <Object>] [-SkipProviderParameters] [-Force]
 [<CommonParameters>]
```

### FilterNames
```
Get-Parameter [-CommandName] <String[]> [[-ParameterName] <String[]>] [-ModuleName <Object>]
 [-SkipProviderParameters] [-Force] [<CommonParameters>]
```

### FilterSets
```
Get-Parameter [-CommandName] <String[]> [-SetName <String[]>] [-ModuleName <Object>] [-SkipProviderParameters]
 [-Force] [<CommonParameters>]
```

## DESCRIPTION
Lists all the parameters of a command, by ParameterSet, including their aliases, type, etc.
By default, formats the output to tables grouped by command and parameter set.

## EXAMPLES

### EXAMPLE 1
```
Get-Command Select-Xml | Get-Parameter
```

### EXAMPLE 2
```
Get-Parameter Select-Xml
```

## PARAMETERS

### -CommandName
The name of the command to get parameters for.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ParameterName
Wilcard-enabled filter for parameter names.

```yaml
Type: System.String[]
Parameter Sets: FilterNames
Aliases:

Required: False
Position: 3
Default value: *
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SetName
The ParameterSet name to filter by (allows wildcards)

```yaml
Type: System.String[]
Parameter Sets: FilterSets
Aliases:

Required: False
Position: Named
Default value: *
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ModuleName
The name of the module which contains the command (this is for scoping)

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SkipProviderParameters
Skip testing for Provider parameters (will be much faster)

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

### -Force
Forces including the CommonParameters in the output.

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
With many thanks to Hal Rottenberg, Oisin Grehan and Shay Levy
Version 0.80 - April 2008 - By Hal Rottenberg http://poshcode.org/186
Version 0.81 - May 2008 - By Hal Rottenberg http://poshcode.org/255
Version 0.90 - June 2008 - By Hal Rottenberg http://poshcode.org/445
Version 0.91 - June 2008 - By Oisin Grehan http://poshcode.org/446
Version 0.92 - April 2008 - By Hal Rottenberg http://poshcode.org/549
             - ADDED resolving aliases and avoided empty output
Version 0.93 - Sept 24, 2009 - By Hal Rottenberg http://poshcode.org/1344
Version 1.0  - Jan 19, 2010 - By Joel Bennett http://poshcode.org/1592
             - Merged Oisin and Hal's code with my own implementation
             - ADDED calculation of dynamic paramters
Version 2.0  - July 22, 2010 - By Joel Bennett http://poshcode.org/get/2005
             - CHANGED uses FormatData so the output is objects
             - ADDED calculation of shortest names to the aliases (idea from Shay Levy http://poshcode.org/1982,
               but with a correct implementation)
Version 2.1  - July 22, 2010 - By Joel Bennett http://poshcode.org/2007
             - FIXED Help for SCRIPT file (script help must be separated from #Requires by an emtpy line)
             - Fleshed out and added dates to this version history after Bergle's criticism ;)
Version 2.2  - July 29, 2010 - By Joel Bennett http://poshcode.org/2030
             - FIXED a major bug which caused Get-Parameters to delete all the parameters from the CommandInfo
Version 2.3  - July 29, 2010 - By Joel Bennett
             - ADDED a ToString ScriptMethod which allows queries like:
               $parameters = Get-Parameter Get-Process; $parameters -match "Name"
Version 2.4  - July 29, 2010 - By Joel Bennett http://poshcode.org/2032
             - CHANGED "Name" to CommandName
             - ADDED ParameterName parameter to allow filtering parameters
             - FIXED bug in 2.3 and 2.2 with dynamic parameters
Version 2.5  - December 13, 2010 - By Jason Archer http://poshcode.org/2404
             - CHANGED format temp file to have static name, prevents bloat of random temporary files
Version 2.6  - July 23, 2011 - By Jason Archer (This Version)
             - FIXED miscalculation of shortest unique name (aliases count as unique names),
               this caused some parameter names to be thrown out (like "Object")
             - CHANGED code style cleanup
Version 2.7  - November 28, 2012 - By Joel Bennett http://poshcode.org/3794
             - Added * indicator on default parameter set.
Version 2.8  - August 27, 2013 - By Joel Bennett (This Version)
             - Added SetName filter
             - Add * on the short name in the aliases list (to distinguish it from real aliases)
             - FIXED PowerShell 4 Bugs:
             - Added PipelineVariable to CommonParameters
             - FIXED PowerShell 3 Bugs:
             - Don't add to the built-in Aliases anymore, it changes the command!
Version 2.9  - July 13, 2015 - By Joel Bennett (This Version)
             - FIXED (hid) exceptions when looking for dynamic parameters
             - CHANGE to only search for provider parameters on Microsoft.PowerShell.Management commands (BUG??)
             - ADDED SkipProviderParameters switch to manually disable looking for provider parameters (faster!)
             - ADDED "Name" alias for CommandName to fix piping Get-Command output

## RELATED LINKS
