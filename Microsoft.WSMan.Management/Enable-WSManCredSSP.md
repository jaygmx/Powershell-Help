---
external help file: Microsoft.WSMan.Management.dll-Help.xml
Module Name: Microsoft.WSMan.Management
online version: https://docs.microsoft.com/powershell/module/microsoft.wsman.management/enable-wsmancredssp?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Enable-WSManCredSSP

## SYNOPSIS
Enables Credential Security Support Provider (CredSSP) authentication on a computer.

## SYNTAX

```
Enable-WSManCredSSP [[-DelegateComputer] <String[]>] [-Force] [-Role] <String> [<CommonParameters>]
```

## DESCRIPTION
\> This cmdlet is only available on the Windows platform.
The \`Enable-WSManCredSSP\` cmdlet enables CredSSP authentication on a client or on a server computer.
When CredSSP authentication is used, the user credentials are passed to a remote computer to be authenticated.
This type of authentication is designed for commands that create a remote session from another remote session.
For example, if you want to run a background job on a remote computer, use this kind of authentication.

\`Enable-WSManCredSSP\` can enable CredSSP on a Client or a Server .
To enable CredSSP on a client, specify Client in the Role parameter.
Clients delegate explicit credentials to a server when server authentication is achieved.
To enable CredSSP on a server, specify Server in the Role parameter.
A server acts as a delegate for clients.
For more details, see Role in the Parameters section.

\> \[!CAUTION\] \> CredSSP authentication delegates the user credentials from the local computer to a remote \> computer.
This practice increases the security risk of the remote operation.
If the remote \> computer is compromised, when credentials are passed to it, the credentials can be used to control \> the network session.

## EXAMPLES

### Example 1: Delegate client credentials
```
Enable-WSManCredSSP -Role "Client" -DelegateComputer "Server02.fabrikam.com"

cfg         : http://schemas.microsoft.com/wbem/wsman/1/config/client/auth
lang        : en-US
Basic       : true
Digest      : true
Kerberos    : true
Negotiate   : true
Certificate : true
CredSSP     : true
```

### Example 2: Delegate client credentials to all computers in a domain
```
Enable-WSManCredSSP -Role "Client" -DelegateComputer "*.fabrikam.com"

cfg         : http://schemas.microsoft.com/wbem/wsman/1/config/client/auth
lang        : en-US
Basic       : true
Digest      : true
Kerberos    : true
Negotiate   : true
Certificate : true
CredSSP     : true
```

### Example 3: Delegate client credentials to multiple computers
```
$servers = "server02.fabrikam.com", "server03.fabrikam.com", "server04.fabrikam.com"
Enable-WSManCredSSP -Role "Client" -DelegateComputer $servers

cfg         : http://schemas.microsoft.com/wbem/wsman/1/config/client/auth
lang        : en-US
Basic       : true
Digest      : true
Kerberos    : true
Negotiate   : true
Certificate : true
CredSSP     : true
```

The \`$servers\` variable contains a list of server names.
\`Enable-WSManCredSSP\` uses the Role parameter to specify the Client role.
The DelegateComputer gets the computer names from the \`$servers\` variable.

### Example 4: Allow a computer to act as a delegate
```
Enable-WSManCredSSP -Role "Server"
```

### Example 5: Allow a computer to act as a delegate by using Set-Item
```
Connect-WSMan -ComputerName "server02"
Set-Item -Path "WSMan:\server02\service\auth\credSSP" -Value $True
```

\`Connect-WSMan\` creates a connection to the remote computer, server02.
\`Set-Item\` uses the Path parameter to specify the WSMan provider's location.
The Value parameter sets the Service setting to true.

## PARAMETERS

### -DelegateComputer
Specifies servers to which client credentials are delegated.
The best practice is to use fully qualified domain names.

Wildcards are accepted, but can enable CredSSP on more computers than necessary.

If the Role parameter is Client , you must specify this parameter.
If Role is Server , don't specify this parameter.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

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

### -Role
Specifies whether to enable CredSSP as a client or as a server.
The acceptable values for this parameter are: Client and Server .

If you specify Client , the following actions are performed.
These settings allow the client to delegate explicit credentials to a server when server authentication is achieved.

- Enables CredSSP on the client.
- Sets the WS-Management setting \`\<localhost|computername\>\Client\Auth\CredSSP\` to true.
- Sets the Windows CredSSP policy AllowFreshCredentials to WSMan/Delegate on the client.

If you specify Server , the following actions are performed.
This policy setting allows the server to act as a delegate for clients.

- Enables CredSSP on the server.
- Sets the WS-Management setting \`\<localhost|computername\>\Service\Auth\CredSSP\` to true.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: Client, Server

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
This cmdlet doesn't accept any input.

## OUTPUTS

### System.Xml.XmlElement
If CredSSP authentication is successfully enabled, this cmdlet generates an XMLElement object.

## NOTES
To disable CredSSP authentication, use the \`Disable-WSManCredSSP\` cmdlet.

## RELATED LINKS

[Connect-WSMan]()

[Disable-WSManCredSSP]()

[Disconnect-WSMan]()

[Get-WSManCredSSP]()

[Get-WSManInstance]()

[Invoke-WSManAction]()

[New-WSManInstance]()

[New-WSManSessionOption]()

[Remove-WSManInstance]()

[Set-WSManInstance]()

[Set-WSManQuickConfig]()

[Test-WSMan]()

