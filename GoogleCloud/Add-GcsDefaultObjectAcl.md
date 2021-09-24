---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GcsDefaultObjectAcl

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### User (Default)
```
Add-GcsDefaultObjectAcl [-Name] <String> -Role <String> -User <String> [<CommonParameters>]
```

### Group
```
Add-GcsDefaultObjectAcl [-Name] <String> -Role <String> -Group <String> [<CommonParameters>]
```

### Domain
```
Add-GcsDefaultObjectAcl [-Name] <String> -Role <String> -Domain <String> [<CommonParameters>]
```

### Team
```
Add-GcsDefaultObjectAcl [-Name] <String> -Role <String> -ProjectNumber <String> -ProjectRole <String>
 [<CommonParameters>]
```

### AllUsers
```
Add-GcsDefaultObjectAcl [-Name] <String> -Role <String> [-AllUsers] [<CommonParameters>]
```

### AllAuthenticatedUsers
```
Add-GcsDefaultObjectAcl [-Name] <String> -Role <String> [-AllAuthenticatedUsers] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -AllAuthenticatedUsers
{{ Fill AllAuthenticatedUsers Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: AllAuthenticatedUsers
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllUsers
{{ Fill AllUsers Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: AllUsers
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Domain
{{ Fill Domain Description }}

```yaml
Type: System.String
Parameter Sets: Domain
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Group
{{ Fill Group Description }}

```yaml
Type: System.String
Parameter Sets: Group
Aliases: GroupId, GroupEmail

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
{{ Fill Name Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Bucket

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectNumber
{{ Fill ProjectNumber Description }}

```yaml
Type: System.String
Parameter Sets: Team
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectRole
{{ Fill ProjectRole Description }}

```yaml
Type: System.String
Parameter Sets: Team
Aliases:
Accepted values: Owners, Editors, Viewers

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Role
{{ Fill Role Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: Reader, Owner

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -User
{{ Fill User Description }}

```yaml
Type: System.String
Parameter Sets: User
Aliases: UserId, UserEmail

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Google.Apis.Storage.v1.Data.ObjectAccessControl

## NOTES

## RELATED LINKS
