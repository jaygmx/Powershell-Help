---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceAddress

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByValues (Default)
```
Add-GceAddress [-Project <String>] [-Region <String>] [-Name] <String> [[-Description] <String>]
 [<CommonParameters>]
```

### ByObject
```
Add-GceAddress [-Project <String>] [-Region <String>] [-Object] <Address> [<CommonParameters>]
```

### GlobalByObject
```
Add-GceAddress [-Project <String>] [-Object] <Address> [-Global] [<CommonParameters>]
```

### GlobalByValues
```
Add-GceAddress [-Project <String>] [-Name] <String> [[-Description] <String>] [-Global] [<CommonParameters>]
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

### -Description
{{ Fill Description Description }}

```yaml
Type: System.String
Parameter Sets: ByValues, GlobalByValues
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Global
{{ Fill Global Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: GlobalByObject, GlobalByValues
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
Parameter Sets: ByValues, GlobalByValues
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
Type: Google.Apis.Compute.v1.Data.Address
Parameter Sets: ByObject, GlobalByObject
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
Parameter Sets: ByValues, ByObject
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

### Google.Apis.Compute.v1.Data.Address

### System.String

## OUTPUTS

### Google.Apis.Compute.v1.Data.Address

## NOTES

## RELATED LINKS
