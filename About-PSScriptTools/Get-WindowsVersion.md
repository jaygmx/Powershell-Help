---
external help file: PSScriptTools-help.xml
Module Name:
online version: http://bit.ly/31QKsTt
schema: 2.0.0
---

# Get-WindowsVersion

## SYNOPSIS
Get Windows version information.

## SYNTAX

```
Get-WindowsVersion [[-Computername] <String[]>] [-Credential <PSCredential>] [-UseSSL] [-ThrottleLimit <Int32>]
 [-Authentication <String>] [<CommonParameters>]
```

## DESCRIPTION
This is a PowerShell version of the winver.exe utility.
This command uses PowerShell remoting to query the registry on a remote machine to retrieve Windows version information.
The parameters are the same as in Invoke-Command.

If you are querying the local computer, all other parameters will be ignored.

## EXAMPLES

### EXAMPLE 1
```
PS C:\>Get-WindowsVersion


   Computername: DESK109

ProductName           EditionID         ReleaseID  Build  InstalledUTC
-----------           ---------         ---------  -----  ------------
Windows 10 Pro        Professional      2009       19042  10/16/2020 3:09:01 PM
```

Query the local host.

### EXAMPLE 2
```
PS C:\> Get-WindowsVersion -Computername srv1,srv2,win10 -Credential $art

   Computername: WIN10

ProductName                EditionID     ReleaseID  Build  InstalledUTC
-----------                ---------     ---------  -----  ------------
Windows 10 Enterprise      Enterprise    1903       18362  2/6/2020 5:28:34 PM


   Computername: SRV1

ProductName                EditionID     ReleaseID  Build  InstalledUTC
-----------                ---------     ---------  -----  ------------
Windows Server 2016        ServerStandard 1607       14393  2/6/2020 5:27:42 PM
Standard


 Computername: SRV2

ProductName                EditionID     ReleaseID  Build  InstalledUTC
-----------                ---------     ---------  -----  ------------
Windows Server 2016        ServerStandard 1607       14393  2/6/2020 6:47:12 PM
Standard
```

Get Windows version information from remote computers using an alternate credential.

### Example 3
```
PS C:\> Get-WindowsVersion -Computername Dom1 | Select-Object *

ProductName  : Windows Server 2016 Standard Evaluation
EditionID    : ServerStandardEval
ReleaseID    : 1607
Build        : 14393.3474
Branch       : rs1_release
InstalledUTC : 2/6/2020 5:18:50 PM
Computername : DOM1
```

## PARAMETERS

### -Computername
Specifies the computers on which the command runs.
The default is the local computer.

When you use the ComputerName parameter, Windows PowerShell creates a temporary connection that is used only to run the specified command and is then closed.
If you need a persistent connection, use the Session parameter.

Type the NETBIOS name, IP address, or fully qualified domain name of one or more computers in a comma-separated list.
To specify the local computer, type the computer name, localhost, or a dot (.).

To use an IP address in the value of ComputerName , the command must include the Credential parameter.
Also, the computer must be configured for HTTPS transport or the IP address of the remote computer must be included in the WinRM TrustedHosts list on the local computer.
For instructions for adding a computer name to the TrustedHosts list, see "How to Add a Computer to the Trusted Host List" in about_Remote_Troubleshooting.

On Windows Vista and later versions of the Windows operating system, to include the local computer in the value of ComputerName , you must open Windows PowerShell by using the Run as administrator option.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: $env:COMPUTERNAME
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Credential
Specifies a user account that has permission to perform this action.
The default is the current user.

Type a user name, such as User01 or Domain01\User01.
Or, enter a PSCredential object, such as one generated by the Get-Credential cmdlet.
If you type a user name, this cmdlet prompts you for a password.

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

### -UseSSL
Indicates that this cmdlet uses the Secure Sockets Layer (SSL) protocol to establish a connection to the remote computer.
By default, SSL is not used.

WS-Management encrypts all Windows PowerShell content transmitted over the network.
The UseSSL parameter is an additional protection that sends the data across an HTTPS, instead of HTTP.

If you use this parameter, but SSL is not available on the port that is used for the command, the command fails.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ThrottleLimit
Specifies the maximum number of concurrent connections that can be established to run this command.
If you omit this parameter or enter a value of 0, the default value, 32, is used.

The throttle limit applies only to the current command, not to the session or to the computer.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Authentication
Specifies the mechanism that is used to authenticate the user's credentials.
The acceptable values for this parameter are:

- Default
- Basic
- Credssp
- Digest
- Kerberos
- Negotiate
- NegotiateWithImplicitCredential

The default value is Default.

CredSSP authentication is available only in Windows Vista, Windows Server 2008, and later versions of the Windows operating system.

For information about the values of this parameter, see the description of the AuthenticationMechanismEnumeration (http://go.microsoft.com/fwlink/?LinkID=144382) in the Microsoft Developer Network (MSDN) library.

CAUTION: Credential Security Support Provider (CredSSP) authentication, in which the user's credentials are passed to a remote computer to be authenticated, is designed for commands that require authentication on more than one resource, such as accessing a remote network share.
This mechanism increases the security risk of the remote operation.
If the remote computer is compromised, the credentials that are passed to it can be used to control the network session.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Default
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
## OUTPUTS

### WindowsVersion
## NOTES
* Learn more about PowerShell: http://jdhitsolutions.com/blog/essential-powershell-resources/

## RELATED LINKS

[Get-WindowsVersionString]()

[WinVer.exe]()

[Invoke-Command]()

