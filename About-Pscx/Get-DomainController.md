---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-DomainController

## SYNOPSIS
PSCX Cmdlet: Gets domain controllers.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-DomainController [[-Name] <String>] [-Credential <PSCredential>] [-Server] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-DomainController [[-Name] <String>] [-Credential <PSCredential>] [-Site] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Get-DomainController [[-Name] <String>] [-Credential <PSCredential>] [-Domain] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_4
```
Get-DomainController [[-Name] <String>] [-Credential <PSCredential>] [-Forest] [<CommonParameters>]
```

## DESCRIPTION
Gets all domain controllers at the specified scope.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
Get-DomainController
```

Gets the domain controller that authenticated the current session.

### EXAMPLE 2
PS C:\\\>

```
Get-DomainController -Domain Europe
```

Gets all domain controllers in the EUROPE domain.

### EXAMPLE 3
PS C:\\\>

```
Get-DomainController -Site
```

Gets all domain controllers in the site this computer is in.

## PARAMETERS

### -Name
Name of the server, site, domain, or forest.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### -Credential
Specifies credentials required to authenticate on the domain controller.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Domain
Returns all domain controllers in the specified domain.
When no domain specified, returns all domain controllers in the current domain.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Forest
Returns all domain controllers in the specified forest.
When no forest specified, returns all domain controllers in the forest.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Server
Returns specified domain controller.
When no server specified, returns the domain controller which authenticated the current session.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Site
Returns all domain controllers in the specified site.
When no site specified, returns all domain controllers in the site this machine is member of.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
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
*

## RELATED LINKS
