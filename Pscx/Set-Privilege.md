---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Set-Privilege

## SYNOPSIS
PSCX Cmdlet: Adjusts privileges associated with a user (identity).

## SYNTAX

```
Set-Privilege [-Privileges] <TokenPrivilegeCollection> [[-Identity] <WindowsIdentity>] [<CommonParameters>]
```

## DESCRIPTION
Adjusts privileges associated with a user (identity).

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
$p = Get-Privilege
$p.Enable('SeTimeZonePrivilege')
Set-Privilege $p
Get-Privilege | ft Name, Status -a

Name Status
---- ------
SeShutdownPrivilege Disabled
SeChangeNotifyPrivilege EnabledByDefault, Enabled
SeUndockPrivilege Disabled
SeIncreaseWorkingSetPrivilege Disabled
SeTimeZonePrivilege Enabled
```

This enables the SeTimeZonePrivilege for the current user.

## PARAMETERS

### -Privileges
The privileges to modify.
See http://msdn.microsoft.com/en-us/library/bb530716(VS.85).aspx for details.

```yaml
Type: Pscx.Interop.TokenPrivilegeCollection
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
The identity to act upon.

```yaml
Type: System.Security.Principal.WindowsIdentity
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
