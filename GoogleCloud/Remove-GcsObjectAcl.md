---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Remove-GcsObjectAcl

## SYNOPSIS


## SYNTAX

### User (Default)
```
Remove-GcsObjectAcl [-Bucket] <String> [-ObjectName] <String> -User <String> [<CommonParameters>]
```

### Group
```
Remove-GcsObjectAcl [-Bucket] <String> [-ObjectName] <String> -Group <String> [<CommonParameters>]
```

### Domain
```
Remove-GcsObjectAcl [-Bucket] <String> [-ObjectName] <String> -Domain <String> [<CommonParameters>]
```

### Team
```
Remove-GcsObjectAcl [-Bucket] <String> [-ObjectName] <String> -ProjectNumber <String> -ProjectRole <String>
 [<CommonParameters>]
```

### AllUsers
```
Remove-GcsObjectAcl [-Bucket] <String> [-ObjectName] <String> [-AllUsers] [<CommonParameters>]
```

### AllAuthenticatedUsers
```
Remove-GcsObjectAcl [-Bucket] <String> [-ObjectName] <String> [-AllAuthenticatedUsers] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -AllAuthenticatedUsers


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

### -Bucket


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Domain


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

### -ObjectName


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectNumber


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

### -User


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

### Google.Apis.Storage.v1.Data.Bucket

## NOTES

## RELATED LINKS
