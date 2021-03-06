---
external help file: AdminToolbox.FileManagement-help.xml
Module Name: AdminToolbox.FileManagement
online version:
schema: 2.0.0
---

# Get-FileOwner

## SYNOPSIS

## SYNTAX

```
Get-FileOwner [-Path] <Object> [-Report] <Object> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
This function produces a CSV listing file owners within a given path

## EXAMPLES

### EXAMPLE 1
```
Specify the parent folder from which all subfolders are queried and where the report should be saved.
```

Get-FileOwner -Path c:\users -Report c:\FileOwners.csv

## PARAMETERS

### -Path
Path where files are to be Audited

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Report
Output path and filename for the report

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

## RELATED LINKS

[Get-ShareNTFSReport
Get-SharePermissionsReport
Find-ComputerFiles]()

