---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-DomainController

## SYNOPSIS
PSCX Cmdlet: Gets domain controllers.

## SYNTAX

### Server (Default)
```
Get-DomainController [[-Name] <String>] [-Server] [-Credential <PSCredential>] [<CommonParameters>]
```

### Site
```
Get-DomainController [[-Name] <String>] [-Site] [-Credential <PSCredential>] [<CommonParameters>]
```

### Domain
```
Get-DomainController [[-Name] <String>] [-Domain] [-Credential <PSCredential>] [<CommonParameters>]
```

### Forest
```
Get-DomainController [[-Name] <String>] [-Forest] [-Credential <PSCredential>] [<CommonParameters>]
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
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Credential
Specifies credentials required to authenticate on the domain controller.

```yaml
Type: System.Management.Automation.PSCredential
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Domain
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Forest
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Server
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Site
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
