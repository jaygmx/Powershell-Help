---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GcdChange

## SYNOPSIS


## SYNTAX

### ChangeRequestSet (Default)
```
Add-GcdChange [-Project <String>] [-Zone] <String> [-ChangeRequest] <Change> [<CommonParameters>]
```

### AddRmSet
```
Add-GcdChange [-Project <String>] [-Zone] <String> [-Add <ResourceRecordSet[]>] [-Remove <ResourceRecordSet[]>]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Add


```yaml
Type: Google.Apis.Dns.v1.Data.ResourceRecordSet[]
Parameter Sets: AddRmSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChangeRequest


```yaml
Type: Google.Apis.Dns.v1.Data.Change
Parameter Sets: ChangeRequestSet
Aliases: Change

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Project


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

### -Remove


```yaml
Type: Google.Apis.Dns.v1.Data.ResourceRecordSet[]
Parameter Sets: AddRmSet
Aliases: Rm

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Zone


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

### Google.Apis.Dns.v1.Data.Change

## OUTPUTS

### Google.Apis.Dns.v1.Data.Change

## NOTES

## RELATED LINKS
