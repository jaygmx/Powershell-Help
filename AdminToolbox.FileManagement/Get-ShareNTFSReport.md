---
external help file: AdminToolbox.FileManagement-help.xml
Module Name: AdminToolbox.FileManagement
online version:
schema: 2.0.0
---

# Get-ShareNTFSReport

## SYNOPSIS

## SYNTAX

```
Get-ShareNTFSReport [[-Path] <Object>] [<CommonParameters>]
```

## DESCRIPTION
Get ntfs permissions for all shares on the local server

## EXAMPLES

### EXAMPLE 1
```
Get-ShareNTFSReport -Path "$env:USERPROFILE\downloads\Group Memberships.xlsx"
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
Default value: "$env:USERPROFILE\downloads\Share NTFS Permissions.xlsx"
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

[Get-SharePermissionsReport
Get-FileOwner
Find-ComputerFiles]()

