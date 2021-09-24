---
external help file: Microsoft.Graph.Authentication.dll-Help.xml
Module Name: Microsoft.Graph.Authentication
online version: https://docs.microsoft.com/en-us/graph/permissions-reference
schema: 2.0.0
---

# Add-MgEnvironment

## SYNOPSIS


## SYNTAX

```
Add-MgEnvironment [-Name] <String> [-AzureADEndpoint] <String> [-GraphEndpoint] <String> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -AzureADEndpoint
The base URL for Azure AD endpoint to get access tokens for Microsoft Graph endpoint.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: AzureADUrl

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GraphEndpoint
The service root endpoint for Microsoft Graph.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: GraphUrl

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
The environment name.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.Graph.PowerShell.Authentication.Models.GraphEnvironment

## NOTES

## RELATED LINKS
