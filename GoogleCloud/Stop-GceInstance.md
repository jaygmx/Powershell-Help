---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Stop-GceInstance

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByName
```
Stop-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> [<CommonParameters>]
```

### ByObject
```
Stop-GceInstance [-Object] <Instance> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Name
{{ Fill Name Description }}

```yaml
Type: System.String
Parameter Sets: ByName
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Object
{{ Fill Object Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.Instance
Parameter Sets: ByObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Project
{{ Fill Project Description }}

```yaml
Type: System.String
Parameter Sets: ByName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Zone
{{ Fill Zone Description }}

```yaml
Type: System.String
Parameter Sets: ByName
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

### System.String

### Google.Apis.Compute.v1.Data.Instance

## OUTPUTS

### Google.Apis.Compute.v1.Data.Instance

## NOTES

## RELATED LINKS
