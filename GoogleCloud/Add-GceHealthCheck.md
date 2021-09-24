---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceHealthCheck

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByValues (Default)
```
Add-GceHealthCheck [-Project <String>] [-Name] <String> [-Description <String>] [-HostHeader <String>]
 [-Port <Int32>] [-RequestPath <String>] [-CheckInterval <TimeSpan>] [-Timeout <TimeSpan>]
 [-HealthyThreshold <Int32>] [-UnhealthyThreshold <Int32>] [-Https] [<CommonParameters>]
```

### ByHttpsObject
```
Add-GceHealthCheck [-Project <String>] [-HttpsObject] <HttpsHealthCheck> [<CommonParameters>]
```

### ByHttpObject
```
Add-GceHealthCheck [-Project <String>] [-HttpObject] <HttpHealthCheck> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -CheckInterval
{{ Fill CheckInterval Description }}

```yaml
Type: System.Nullable`1[System.TimeSpan]
Parameter Sets: ByValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
{{ Fill Description Description }}

```yaml
Type: System.String
Parameter Sets: ByValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HealthyThreshold
{{ Fill HealthyThreshold Description }}

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: ByValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HostHeader
{{ Fill HostHeader Description }}

```yaml
Type: System.String
Parameter Sets: ByValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HttpObject
{{ Fill HttpObject Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.HttpHealthCheck
Parameter Sets: ByHttpObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Https
{{ Fill Https Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ByValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HttpsObject
{{ Fill HttpsObject Description }}

```yaml
Type: Google.Apis.Compute.v1.Data.HttpsHealthCheck
Parameter Sets: ByHttpsObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
{{ Fill Name Description }}

```yaml
Type: System.String
Parameter Sets: ByValues
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Port
{{ Fill Port Description }}

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: ByValues
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

### -RequestPath
{{ Fill RequestPath Description }}

```yaml
Type: System.String
Parameter Sets: ByValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Timeout
{{ Fill Timeout Description }}

```yaml
Type: System.Nullable`1[System.TimeSpan]
Parameter Sets: ByValues
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UnhealthyThreshold
{{ Fill UnhealthyThreshold Description }}

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: ByValues
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

### Google.Apis.Compute.v1.Data.HttpsHealthCheck

### Google.Apis.Compute.v1.Data.HttpHealthCheck

## OUTPUTS

### Google.Apis.Compute.v1.Data.HttpHealthCheck

### Google.Apis.Compute.v1.Data.HttpsHealthCheck

## NOTES

## RELATED LINKS
