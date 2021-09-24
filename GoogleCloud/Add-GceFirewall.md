---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceFirewall

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
Add-GceFirewall [-Project <String>] [-Name] <String>
 -AllowedProtocol <System.Collections.Generic.List`1[Google.Apis.Compute.v1.Data.Firewall+AllowedData]>
 [-Description <String>] [-Network <String>] [-SourceRange <System.Collections.Generic.List`1[System.String]>]
 [-SourceTag <System.Collections.Generic.List`1[System.String]>]
 [-TargetTag <System.Collections.Generic.List`1[System.String]>] [<CommonParameters>]
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

### -AllowedProtocol
{{ Fill AllowedProtocol Description }}

```yaml
Type: System.Collections.Generic.List`1[Google.Apis.Compute.v1.Data.Firewall+AllowedData]
Parameter Sets: (All)
Aliases: Allowed, Protocol

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Description
{{ Fill Description Description }}

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

### -Name
{{ Fill Name Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Network
{{ Fill Network Description }}

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

### -SourceRange
{{ Fill SourceRange Description }}

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceTag
{{ Fill SourceTag Description }}

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetTag
{{ Fill TargetTag Description }}

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
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

### System.Collections.Generic.List`1[[Google.Apis.Compute.v1.Data.Firewall+AllowedData, Google.Apis.Compute.v1, Version=1.29.1.981, Culture=neutral, PublicKeyToken=4b01fa6e34db77ab]]

## OUTPUTS

### Google.Apis.Compute.v1.Data.Firewall

## NOTES

## RELATED LINKS
