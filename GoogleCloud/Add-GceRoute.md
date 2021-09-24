---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceRoute

## SYNOPSIS


## SYNTAX

### FromObject
```
Add-GceRoute [-Project <String>] [-Object] <Route> [<CommonParameters>]
```

### FromValues
```
Add-GceRoute [-Project <String>] [-Name] <String> [-DestinationIpRange] <String> [-Network] <String>
 [-Priority <Int64>] [-Description <String>] [-Tag <String[]>] [-NextHopInstance <String>]
 [-NextHopIp <String>] [-NextHopVpnTunnel <String>] [-NextHopInternetGateway] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Description


```yaml
Type: System.String
Parameter Sets: FromValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestinationIpRange


```yaml
Type: System.String
Parameter Sets: FromValues
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name


```yaml
Type: System.String
Parameter Sets: FromValues
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Network


```yaml
Type: System.String
Parameter Sets: FromValues
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NextHopInstance


```yaml
Type: System.String
Parameter Sets: FromValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NextHopInternetGateway


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FromValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NextHopIp


```yaml
Type: System.String
Parameter Sets: FromValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NextHopVpnTunnel


```yaml
Type: System.String
Parameter Sets: FromValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Object


```yaml
Type: Google.Apis.Compute.v1.Data.Route
Parameter Sets: FromObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Priority


```yaml
Type: System.Nullable`1[System.Int64]
Parameter Sets: FromValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### -Tag


```yaml
Type: System.String[]
Parameter Sets: FromValues
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

### Google.Apis.Compute.v1.Data.Route

## OUTPUTS

### Google.Apis.Compute.v1.Data.Route

## NOTES

## RELATED LINKS
