---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-PscxADObject

## SYNOPSIS
PSCX Cmdlet: Search for objects in the Active Directory/Global Catalog.

## SYNTAX

```
Get-PscxADObject [-Class <ObjectClass[]>] [-Credential <PSCredential>] [-DistinguishedName <String>]
 [-Domain <String>] [-Filter <String>] [-GlobalCatalog] [-PageSize <Int32>] [-Scope <SearchScope>]
 [-Server <String>] [-SizeLimit <Int32>] [-Value <String>] [<CommonParameters>]
```

## DESCRIPTION
Search for objects in the Active Directory/Global Catalog.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
PS> Get-PsxcADObject -domain example.com -class user
```

This command displays all Active Directory user from the domain example.com.

### EXAMPLE 2
PS C:\\\>

```
PS> Get-PsxcADObject -value "*user*"
```

This command returns all Active Directory objects that contain the word "user".

### EXAMPLE 3
PS C:\\\>

```
PS> Get-PsxcADObject -filter "(&(mail=*user*)(sn=*user*))"
```

This command returns all Active Directory objects that contain the word "user"
        within the e-mail and surename fields.

## PARAMETERS

### -Class
Result returns only objects form the selected classes.

```yaml
Type: ObjectClass[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
Specifies credentials required to authenticate on the domain controller.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DistinguishedName
Specify the search path (Format: distinguished name  e.g.
"DC=some,DC=domain,DC=xx")

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Domain
Specify the domain name for the search.
(Format: canonical name  e.g.
some.domain.xx)

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Logon domain from the user.
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filter
Specify the search filter

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GlobalCatalog
Use Global Catalog for the search

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PageSize
@{Text=}

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Scope
Search scope

```yaml
Type: SearchScope
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Subtree
Accept pipeline input: False
Accept wildcard characters: False
```

### -Server
Send the request to this active directory domain controller.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SizeLimit
@{Text=}

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value
Search string.
Wildcards are permitted.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

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
* 
        Using this cmdlet without a parameter will return all Active Directory objects from
        the current domain. Depending on the size of the logon domain this operation can take
        longer.

## RELATED LINKS
