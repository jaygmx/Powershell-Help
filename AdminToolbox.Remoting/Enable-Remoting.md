---
external help file: AdminToolbox.Remoting-help.xml
Module Name: AdminToolbox.Remoting
online version:
schema: 2.0.0
---

# Enable-Remoting

## SYNOPSIS

## SYNTAX

```
Enable-Remoting [-Computer] <Object> [[-Username] <Object>] [[-Password] <SecureString>] [<CommonParameters>]
```

## DESCRIPTION
This Command will enable PowerShell Remoting on a remote PC.

## EXAMPLES

### EXAMPLE 1
```
This will enable remoting and then prompt for credentials
```

Enable-PSRemoting -computer PCName -username domain\username

## PARAMETERS

### -Computer
Computer that PSRemoting is being enabled on

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

### -Username
Username used by PSExec to authenticate with admin privleges

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Password
Password that is associated with the username used

```yaml
Type: System.Security.SecureString
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
This function requires psexec.
If you do not, download it with the sysinternals suite.
Add psexec to one of your enviroment variable paths.

## RELATED LINKS
