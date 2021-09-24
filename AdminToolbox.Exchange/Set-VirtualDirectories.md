---
external help file: AdminToolbox.Exchange-help.xml
Module Name: AdminToolbox.Exchange
online version:
schema: 2.0.0
---

# Set-VirtualDirectories

## SYNOPSIS

## SYNTAX

```
Set-VirtualDirectories [-servername] <Object> [-url] <Object> [<CommonParameters>]
```

## DESCRIPTION
Configure Virtual Directories for Exchange

## EXAMPLES

### EXAMPLE 1
```
Specify the mail server directories are being set on and the url that matches the mail records.
```

Set-VirtualDirectories -Servername exch2016-01 -url mail.domain.com

## PARAMETERS

### -servername
Server that the directories are being set on

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

### -url
Domail specific url being set for the virtual directories

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-VirtualDirectories]()

