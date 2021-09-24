---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# Stop-RemoteProcess

## SYNOPSIS
Stops a process on a remote machine.

## SYNTAX

### Name
```
Stop-RemoteProcess [-ComputerName] <String> [-Name] <String[]> [-Credential <PSCredential>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Id
```
Stop-RemoteProcess [-ComputerName] <String> [-Id] <Int32[]> [-Credential <PSCredential>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Stops a process on a remote machine.
This command uses WMI to terminate the remote process.

## EXAMPLES

### EXAMPLE 1
```
Stop-RemoteProcess server1 notepad.exe
Stops all processes named notepad.exe on the remote computer server1.
```

### EXAMPLE 2
```
Stop-RemoteProcess server1 3478
Stops the process with process id 3478 on the remote computer server1.
```

### EXAMPLE 3
```
3478,4005 | Stop-RemoteProcess server1
Stops the processes with process ids 3478 and 4005 on the remote computer server1.
```

## PARAMETERS

### -ComputerName
The name of the remote computer that the process is executing on.
Type the NetBIOS name, an IP address, or a fully qualified domain name of the remote computer.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The process name of the remote process to terminate.

```yaml
Type: System.String[]
Parameter Sets: Name
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Id
The process id of the remote process to terminate.

```yaml
Type: System.Int32[]
Parameter Sets: Id
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Credential
Specifies a user account that has permission to perform this action.
The default is the current user.
Type a user name, such as "User01", "Domain01\User01", or User@Contoso.com.
Or, enter a PSCredential
object, such as an object that is returned by the Get-Credential cmdlet.
When you type a user name,
you will be prompted for a password.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Jachym Kouba and Keith Hill

## RELATED LINKS
