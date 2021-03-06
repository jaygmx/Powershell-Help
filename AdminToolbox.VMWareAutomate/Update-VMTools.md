---
external help file: AdminToolbox.VMWareAutomate-help.xml
Module Name: AdminToolbox.VMWareAutomate
online version:
schema: 2.0.0
---

# Update-VMTools

## SYNOPSIS

## SYNTAX

```
Update-VMTools [-Unmanaged] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Filter out 2003 servers and upgrade VMwaretools on all servers that are not up to date.
Does not reboot the VM's.

## EXAMPLES

### EXAMPLE 1
```
Upgrades only tools that are installed an require it. Specify a path for a log file.
```

Update-VMTools

### EXAMPLE 2
```
Include unmanaged VM's
```

Update-VMTools -Unmanaged

## PARAMETERS

### -Unmanaged
Specifies if vmtools should be installd on VM's that don't have them installed.

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
Requires the VMware.PowerCLI Module

## RELATED LINKS

[Get-VMTools]()

