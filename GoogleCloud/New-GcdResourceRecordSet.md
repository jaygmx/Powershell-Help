---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcdResourceRecordSet

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
New-GcdResourceRecordSet [-Name] <String> [-Rrdata] <String[]> [-Type] <String> [[-Ttl] <Int32>]
 [<CommonParameters>]
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
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Rrdata
{{ Fill Rrdata Description }}

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: Data

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Ttl
{{ Fill Ttl Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
{{ Fill Type Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: A, AAAA, CNAME, MX, NAPTR, NS, PTR, SOA, SPF, SRV, TXT

Required: True
Position: 2
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
