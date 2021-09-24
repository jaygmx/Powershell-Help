---
external help file: AdminToolbox.FileManagement-help.xml
Module Name: AdminToolbox.FileManagement
online version:
schema: 2.0.0
---

# Get-SharePermissionsReport

## SYNOPSIS

## SYNTAX

```
Get-SharePermissionsReport [[-Path] <Object>] [<CommonParameters>]
```

## DESCRIPTION
Get share permissions for all shares on the local server

## EXAMPLES

### EXAMPLE 1
```
Get-ShareNTFSReport -Path "$env:USERPROFILE\downloads\Share Permissions.xlsx"
```

## PARAMETERS

### -Path
Specifies the export directory and filename for the report

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: "$env:USERPROFILE\downloads\Share Permissions.xlsx"
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Requires Active Directory and ImportExcel Modules

## RELATED LINKS

[Get-ShareNTFSReport
Get-FileOwner
Find-ComputerFiles]()

