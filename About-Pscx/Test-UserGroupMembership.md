---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Test-UserGroupMembership

## SYNOPSIS
PSCX Cmdlet: Tests whether or not a user (current user by default) is a member of the specified group name.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Test-UserGroupMembership [-GroupName] <String[]> [[-Identity] <WindowsIdentity>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Test-UserGroupMembership [-IdentityReference] <IdentityReference[]> [[-Identity] <WindowsIdentity>]
 [<CommonParameters>]
```

## DESCRIPTION
Tests whether or not a user (current user by default) is a member of the specified group name. 
This can be used to test whether a user is admin or elevated to admin.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
PS> Test-UserGroupMembership -GroupName Administrators
False
```

Tests to see if the current user is a member of the Administrators group.

## PARAMETERS

### -GroupName
Name of the group to test membership of.
Examples: Administrators, Users, Power Users, etc

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IdentityReference
Reference to the identity to act upon.

```yaml
Type: IdentityReference[]
Parameter Sets: UNNAMED_PARAMETER_SET_2
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
Type: WindowsIdentity
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

### Boolean
## NOTES
*

## RELATED LINKS
