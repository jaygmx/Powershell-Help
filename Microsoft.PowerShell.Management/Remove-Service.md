---
external help file: Microsoft.PowerShell.Commands.Management.dll-Help.xml
Module Name: Microsoft.PowerShell.Management
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.management/remove-service?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Remove-Service

## SYNOPSIS
Removes a Windows service.

## SYNTAX

### Name (Default)
```
Remove-Service [-Name] <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### InputObject
```
Remove-Service [-InputObject <ServiceController>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The \`Remove-Service\` cmdlet removes a Windows service in the registry and in the service database.

The \`Remove-Service\` cmdlet was introduced in PowerShell 6.0.

## EXAMPLES

### Example 1: Remove a service
```
Remove-Service -Name "TestService"
```

### Example 2: Remove a service using the display name
```
Get-Service -DisplayName "Test Service" | Remove-Service
```

## PARAMETERS

### -InputObject
Specifies ServiceController objects that represent the services to remove.
Enter a variable that contains the objects, or type a command or expression that gets the objects.

The InputObject parameter doesn't enumerate collections.
If a collection is passed, an error is thrown.
When working with collections, pipe the input to enumerate the values.

```yaml
Type: System.ServiceProcess.ServiceController
Parameter Sets: InputObject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the service names of the services to remove.
Wildcard characters are permitted.

```yaml
Type: System.String
Parameter Sets: Name
Aliases: ServiceName, SN

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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
Default value: False
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
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.ServiceProcess.ServiceController, System.String
You can pipe a service object or a string that contains the name of a service to this cmdlet.

## OUTPUTS

### None
This cmdlet does not return any output.

## NOTES
This cmdlet is only available on Windows platforms.

To run this cmdlet, start PowerShell by using the Run as administrator option.

## RELATED LINKS

[Get-Service]()

[Restart-Service]()

[Resume-Service]()

[Set-Service]()

[Start-Service]()

[Stop-Service]()

[Suspend-Service]()

