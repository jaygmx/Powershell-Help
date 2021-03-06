---
external help file: AdminToolbox.EndpointManagement-help.xml
Module Name: AdminToolbox.EndpointManagement
online version:
schema: 2.0.0
---

# Reset-EndpointPassword

## SYNOPSIS

## SYNTAX

```
Reset-EndpointPassword [-Server] <Object> [-User] <Object> [<CommonParameters>]
```

## DESCRIPTION
This function rebuilds the trust relationship for a workstation or server to a Domain

## EXAMPLES

### EXAMPLE 1
```
Reaches out to a specified domain controller using a domain admin account to rebuild the trust relationship
```

Reset-EndpintPassword CompanyDC01 Domain\Username

## PARAMETERS

### -Server
Used to specify a domain controller in the domain

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -User
Used to specify a domain admin account

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
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
