---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Set-GceTargetPool

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### RemoveInstanceByName
```
Set-GceTargetPool [-Project <String>] [-Region <String>] [-Name] <String> -RemoveInstance <String[]>
 [<CommonParameters>]
```

### AddInstanceByName
```
Set-GceTargetPool [-Project <String>] [-Region <String>] [-Name] <String> -AddInstance <String[]>
 [<CommonParameters>]
```

### RemoveInstanceByObject
```
Set-GceTargetPool -InputObject <TargetPool> -RemoveInstance <String[]> [<CommonParameters>]
```

### AddInstanceByObject
```
Set-GceTargetPool -InputObject <TargetPool> -AddInstance <String[]> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -AddInstance
{{ Fill AddInstance Description }}

```yaml
Type: System.String[]
Parameter Sets: AddInstanceByName, AddInstanceByObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
{{ Fill InputObject Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.TargetPool
Parameter Sets: RemoveInstanceByObject, AddInstanceByObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
{{ Fill Name Description }}

```yaml
Type: System.String
Parameter Sets: RemoveInstanceByName, AddInstanceByName
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Project
{{ Fill Project Description }}

```yaml
Type: System.String
Parameter Sets: RemoveInstanceByName, AddInstanceByName
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
Parameter Sets: RemoveInstanceByName, AddInstanceByName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveInstance
{{ Fill RemoveInstance Description }}

```yaml
Type: System.String[]
Parameter Sets: RemoveInstanceByName, RemoveInstanceByObject
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

### Google.Apis.Compute.v1.Data.TargetPool

## OUTPUTS

### Google.Apis.Compute.v1.Data.TargetPool

## NOTES

## RELATED LINKS
