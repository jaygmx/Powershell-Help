---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Get-GcSqlSslCert

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### Single
```
Get-GcSqlSslCert [-Project <String>] [-Instance] <String> [-Sha1Fingerprint] <String> [<CommonParameters>]
```

### List
```
Get-GcSqlSslCert [-Project <String>] [-Instance] <String> [<CommonParameters>]
```

### List from Instance
```
Get-GcSqlSslCert [-Project <String>] -InstanceObject <DatabaseInstance> [<CommonParameters>]
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

### -Instance
{{ Fill Instance Description }}

```yaml
Type: System.String
Parameter Sets: Single, List
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstanceObject
{{ Fill InstanceObject Description }}

```yaml
Type: Google.Apis.SQLAdmin.v1beta4.Data.DatabaseInstance
Parameter Sets: List from Instance
Aliases:

Required: True
Position: Named
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

### -Sha1Fingerprint
{{ Fill Sha1Fingerprint Description }}

```yaml
Type: System.String
Parameter Sets: Single
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.SQLAdmin.v1beta4.Data.DatabaseInstance

## OUTPUTS

### Google.Apis.SQLAdmin.v1beta4.Data.SslCert

## NOTES

## RELATED LINKS
