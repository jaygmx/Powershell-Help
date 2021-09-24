---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Get-GceImage

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### OfProject (Default)
```
Get-GceImage [[-Project] <String[]>] [-IncludeDeprecated] [<CommonParameters>]
```

### ByName
```
Get-GceImage [-Name] <String> [[-Project] <String[]>] [<CommonParameters>]
```

### ByFamily
```
Get-GceImage -Family <String> [[-Project] <String[]>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Family
{{ Fill Family Description }}

```yaml
Type: System.String
Parameter Sets: ByFamily
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeDeprecated
{{ Fill IncludeDeprecated Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: OfProject
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -Project
{{ Fill Project Description }}

```yaml
Type: System.String[]
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

### System.String

## OUTPUTS

### Google.Apis.Compute.v1.Data.Image

## NOTES

## RELATED LINKS
