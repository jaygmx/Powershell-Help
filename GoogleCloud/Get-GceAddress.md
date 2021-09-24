---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Get-GceAddress

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### OfProject (Default)
```
Get-GceAddress [-Project <String>] [<CommonParameters>]
```

### OfRegion
```
Get-GceAddress [-Project <String>] -Region <String> [<CommonParameters>]
```

### ByName
```
Get-GceAddress [-Project <String>] [-Region <String>] [-Name] <String> [<CommonParameters>]
```

### Global
```
Get-GceAddress [-Project <String>] [-Global] [<CommonParameters>]
```

### GlobalByName
```
Get-GceAddress [-Project <String>] [-Name] <String> [-Global] [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Global
{{ Fill Global Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Global, GlobalByName
Aliases:

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
Parameter Sets: ByName, GlobalByName
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
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Region
{{ Fill Region Description }}

```yaml
Type: System.String
Parameter Sets: OfRegion
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

## OUTPUTS

### Google.Apis.Compute.v1.Data.Address

## NOTES

## RELATED LINKS
