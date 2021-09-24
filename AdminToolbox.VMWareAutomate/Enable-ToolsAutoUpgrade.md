---
external help file: AdminToolbox.VMWareAutomate-help.xml
Module Name: AdminToolbox.VMWareAutomate
online version:
schema: 2.0.0
---

# Enable-ToolsAutoUpgrade

## SYNOPSIS

## SYNTAX

```
Enable-ToolsAutoUpgrade [-Unmanaged] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Filter out 2003 servers and servers that don't have Vmware Tools installed.

All remaining servers will have their tools set to upgrade automatically.

## EXAMPLES

### EXAMPLE 1
```
Enable-ToolsAutoUpgrade
```

### EXAMPLE 2
```
Include VM's Without Guest Tools Installed
```

Enable-ToolsAutoUpgrade -Unmanaged

## PARAMETERS

### -Unmanaged
Specifies VM's without tools installed that should have AutoUpgrade enabled.

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

[Get-ToolsAutoUpgrade]()

