---
external help file: Microsoft.Graph.Authentication-help.xml
Module Name: Microsoft.Graph.Authentication
online version:
schema: 2.0.0
---

# Find-MgGraphCommand

## SYNOPSIS
Find Microsoft Graph PowerShell command meta-info by URI or command name.

## SYNTAX

### FindByUri (Default)
```
Find-MgGraphCommand [-Uri] <String[]> [-Method <String>] [-ApiVersion <String>] [<CommonParameters>]
```

### FindByCommand
```
Find-MgGraphCommand [-ApiVersion <String>] -Command <String[]> [<CommonParameters>]
```

## DESCRIPTION
The Find-MgGraphCommand command retrieves meta-info about Microsoft Graph PowerShell commands by URI or command name.

## EXAMPLES

### EXAMPLE 1
```
Find-MgGraphCommand -Uri "/users/{id}"
```

APIVersion: v1.0

Command       Module Method URI              OutputType           Permissions
-------       ------ ------ ---              ----------           -----------
Get-MgUser    Users  GET    /users/{user-id} IMicrosoftGraphUser1 {DeviceManagementApps.Read.All DeviceManagementApps.Rea…
Remove-MgUser Users  DELETE /users/{user-id}                      {DeviceManagementApps.ReadWrite.All DeviceManagementMan…
Update-MgUser Users  PATCH  /users/{user-id}                      {DeviceManagementApps.ReadWrite.All DeviceManagementMan…

   APIVersion: beta

Command       Module Method URI              OutputType          Permissions
-------       ------ ------ ---              ----------          -----------
Get-MgUser    Users  GET    /users/{user-id} IMicrosoftGraphUser {DeviceManagementApps.Read.All DeviceManagementApps.Read…
Remove-MgUser Users  DELETE /users/{user-id}                     {DeviceManagementApps.ReadWrite.All DeviceManagementMana…
Update-MgUser Users  PATCH  /users/{user-id}                     {DeviceManagementApps.ReadWrite.All DeviceManagementMana…

This example finds all commands that call the provided Microsoft Graph URI.

### EXAMPLE 2
```
Find-MgGraphCommand -Command Send-MgUserMessage -ApiVersion beta
```

APIVersion: beta

Command            Module        Method URI                                                         OutputType Permissions
-------            ------        ------ ---                                                         ---------- -----------
Send-MgUserMessage Users.Actions POST   /users/{user-id}/messages/{message-id}/microsoft.graph.send            {Mail.Send}

This example looks up a command with the provided command name that calls the beta version of the API.

## PARAMETERS

### -Uri
The API path a command calls.
e.g., /users.

```yaml
Type: System.String[]
Parameter Sets: FindByUri
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Method
The HTTP method a command makes.

```yaml
Type: System.String
Parameter Sets: FindByUri
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApiVersion
The service API version.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Profile

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Command
The name of a command.
e.g., Get-MgUser.

```yaml
Type: System.String[]
Parameter Sets: FindByCommand
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Pipeline input accepts API URIs as an array of strings.
## OUTPUTS

### Microsoft.Graph.PowerShell.Authentication.Models.IGraphCommand with the following properties:
###     1. Command: Name of command.
###     2. Module: Module in which a command is defined.
###     3. Method: The HTTP method a command makes.
###     4. Uri: The Microsoft Graph API URI a command calls.
###     5. OutputType: The return type of a command.
###     6. Permissions: Permissions needed to use a command. This field can be empty if the permissions are not yet available in Graph Explorer.
###     7. Variants: The parameter sets of a command.
## NOTES

## RELATED LINKS
