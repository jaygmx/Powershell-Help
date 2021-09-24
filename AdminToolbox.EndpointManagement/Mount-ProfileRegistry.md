---
external help file: AdminToolbox.EndpointManagement-help.xml
Module Name: AdminToolbox.EndpointManagement
online version:
schema: 2.0.0
---

# Mount-ProfileRegistry

## SYNOPSIS

## SYNTAX

```
Mount-ProfileRegistry [-SamAccountName] <Object> [[-DomainController] <Object>] [<CommonParameters>]
```

## DESCRIPTION
Loads any local users registry hive into the registry as a friendly name.
Useful for modifying a users registry without the need of them being logged in locally.

## EXAMPLES

### EXAMPLE 1
```
If you have the AD module locally installed there is no need to specify the domain controller.
```

Mount-ProfileRegistry -SamAccountName JohnS

### EXAMPLE 2
```
Specify the domain controller to implicitly import the active directory module from a Domain Controller with Powershell Remoting.
```

Mount-ProfileRegistry -SamAccountName JohnS -DomainController TexasDC2016

## PARAMETERS

### -SamAccountName
SamAccountName of the domain account that you are mounting the local registry for.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DomainController
Domain Controller that has Powershell Remoting enabled on it.
For importing a session with the Active directory Module.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
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

[DisMount-ProfileRegistry]()

