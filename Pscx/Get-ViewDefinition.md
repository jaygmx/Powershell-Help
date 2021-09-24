---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-ViewDefinition

## SYNOPSIS
Gets the possible alternate views for the specified object.

## SYNTAX

### Name (Default)
```
Get-ViewDefinition [[-TypeName] <String>] [[-Path] <String[]>] [-IncludeSnapInFormatting] [<CommonParameters>]
```

### Object
```
Get-ViewDefinition [[-InputObject] <PSObject>] [[-Path] <String[]>] [-IncludeSnapInFormatting]
 [<CommonParameters>]
```

## DESCRIPTION
Gets the possible alternate views for the specified object.

## EXAMPLES

### EXAMPLE 1
```
Get-ViewDefinition
Retrieves all view definitions from the PowerShell format files.
```

### EXAMPLE 2
```
Get-ViewDefinition System.Diagnostics.Process
Retrieves all view definitions for the .NET type System.Diagnostics.Process.
```

### EXAMPLE 3
```
Get-Process | Get-ViewDefinition | ft Name,Style -groupby SelectedBy
Retrieves all view definitions for the .NET type System.Diagnostics.Process.
```

### EXAMPLE 4
```
Get-ViewDefinition Pscx.Commands.Net.PingHostStatistics $Pscx:Home\Modules\Net\Pscx.Net.Format.ps1xml
Retrieves all view definitions for the .NET type Pscx.Commands.Net.PingHostStatistics.
```

## PARAMETERS

### -TypeName
Name of the type for which to retrieve the view definitions.

```yaml
Type: System.String
Parameter Sets: Name
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
{{ Fill InputObject Description }}

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: Object
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Path
Path to a specific format data PS1XML file. 
Wildcards are accepted. 
The default
value is an empty array which will load the default .ps1xml files and exported
format files from modules loaded in the current session

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: @()
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeSnapInFormatting
Include the exported format information from v1 PSSnapins.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Joris van Lier and Keith Hill

## RELATED LINKS
