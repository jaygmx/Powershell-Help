---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceRoute

## SYNOPSIS
{{ Fill in the Synopsis }}

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
Parameter Sets: FromValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestinationIpRange
{{ Fill DestinationIpRange Description }}

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
{{ Fill Name Description }}

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
{{ Fill Network Description }}

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
{{ Fill NextHopInstance Description }}

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
{{ Fill NextHopInternetGateway Description }}

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
{{ Fill NextHopIp Description }}

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
{{ Fill NextHopVpnTunnel Description }}

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
{{ Fill Object Description }}

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
{{ Fill Priority Description }}

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

### -Tag
{{ Fill Tag Description }}

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
