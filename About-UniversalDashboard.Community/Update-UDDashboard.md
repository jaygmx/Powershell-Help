---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# Update-UDDashboard

## SYNOPSIS
Updates a running dashboard.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Update-UDDashboard [-AllowTLs10] -Content <ScriptBlock> -UpdateToken <Object> -Url <Object>
 [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Update-UDDashboard [-AllowTLs10] -FilePath <String> -UpdateToken <Object> -Url <Object> [<CommonParameters>]
```

## DESCRIPTION
Updates a running dashboard.
To be able to support this cmdlet you need to specify the UpdateToken parameter on Start-UDDashboard.

## EXAMPLES

### Example 1
```
PS C:\> Start-UDDashboard -UpdateToken 1234 -Port 8080
PS C:\> Update-UDDashboard -UpdateToken 1234 -Url http://localhost:8080 -Content {
    New-UDDashboard -Title "Updated" -Content {
        New-UDCard -TItle "Updated Content"
    }
}
```

Starts a dashboard and updates it using Update-UDDashboard.

## PARAMETERS

### -AllowTLs10
Allows TLS 1.0 for the web request.

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

### -Content
The content of the dashboard to update.

```yaml
Type: ScriptBlock
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FilePath
The file path of a PS1 that returns a New-UDDashboard.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UpdateToken
The update token for the dashboard.
This is specified with Start-UDDashboard.
Treat this as a password.

```yaml
Type: Object
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Url
The URL of the running Universal Dashboard.

```yaml
Type: Object
Parameter Sets: (All)
Aliases:

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

### System.Object
## NOTES
*

## RELATED LINKS
