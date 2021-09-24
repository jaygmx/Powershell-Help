---
external help file: AdminToolbox.EndpointManagement-help.xml
Module Name: AdminToolbox.EndpointManagement
online version:
schema: 2.0.0
---

# Install-ChocoPackages

## SYNOPSIS

## SYNTAX

```
Install-ChocoPackages [-Install] <Object> [<CommonParameters>]
```

## DESCRIPTION
Install one or Multiple Choclatey Packages

## EXAMPLES

### EXAMPLE 1
```
Install a single application
```

Install-ChocoPackages -install firefox

### EXAMPLE 2
```
Install Multiple Applications.
```

Install-ChocoPackages -install firefox, chrome, nmap

## PARAMETERS

### -Install
Specify applications to install

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
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

[Get-ChocoInstalls
Get-ChocoOutdated
Install-Chocolatey
Invoke-ChocoUpgrade]()

