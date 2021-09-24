---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GceFirewallProtocol

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### Default (Default)
```
New-GceFirewallProtocol [-IPProtocol] <String> [-Port <System.Collections.Generic.List`1[System.String]>]
 [<CommonParameters>]
```

### AppendPipeline
```
New-GceFirewallProtocol [-IPProtocol] <String> [-Port <System.Collections.Generic.List`1[System.String]>]
 [-Pipeline <Object>] [<CommonParameters>]
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

### -IPProtocol
{{ Fill IPProtocol Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Protocol

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Pipeline
{{ Fill Pipeline Description }}

```yaml
Type: System.Object
Parameter Sets: AppendPipeline
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Port
{{ Fill Port Description }}

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

### System.Object

## OUTPUTS

### Google.Apis.Compute.v1.Data.Firewall+AllowedData

## NOTES

## RELATED LINKS
