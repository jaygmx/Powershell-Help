---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Get-GcdResourceRecordSet

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
Get-GcdResourceRecordSet [-Project <String>] [-Zone] <String> [[-Filter] <String[]>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Filter
{{ Fill Filter Description }}

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:
Accepted values: A, AAAA, CNAME, MX, NAPTR, NS, PTR, SOA, SPF, SRV, TXT

Required: False
Position: 1
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

### -Zone
{{ Fill Zone Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: ManagedZone

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Google.Apis.Dns.v1.Data.ResourceRecordSet

## NOTES

## RELATED LINKS
