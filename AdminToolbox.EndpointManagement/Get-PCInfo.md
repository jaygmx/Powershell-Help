---
external help file: AdminToolbox.EndpointManagement-help.xml
Module Name: AdminToolbox.EndpointManagement
online version:
schema: 2.0.0
---

# Get-PCInfo

## SYNOPSIS

## SYNTAX

```
Get-PCInfo [[-Computer] <Object>] [<CommonParameters>]
```

## DESCRIPTION
Returns useful informaion on the local endpoint or another.

## EXAMPLES

### EXAMPLE 1
```
Returns PCinfo for the local computer
```

Get-PCinfo

### EXAMPLE 2
```
Returns PCinfo for a remote computer
```

Get-PCinfo -computer PCName

## PARAMETERS

### -Computer
Specify a remote computer to get info for

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Requires Powershell 5.1

## RELATED LINKS

[Get-ADInfo]()

