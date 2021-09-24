---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Add-GceManagedInstanceGroup

## SYNOPSIS


## SYNTAX

### ByZoneProperties (Default)
```
Add-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Name] <String> [-InstanceTemplate] <String>
 [-TargetSize] <Int32> [-BaseInstanceName <String>] [-Description <String>] [-TargetPool <String[]>]
 [-PortName <String[]>] [-PortNumber <Int32[]>] [-NamedPort <NamedPort[]>] [<CommonParameters>]
```

### ByObject
```
Add-GceManagedInstanceGroup [-Project <String>] [-Zone <String>] [-Region <String>]
 [-Object] <InstanceGroupManager> [<CommonParameters>]
```

### ByRegionProperties
```
Add-GceManagedInstanceGroup [-Project <String>] [-Region <String>] [-Name] <String>
 [-InstanceTemplate] <String> [-TargetSize] <Int32> [-BaseInstanceName <String>] [-Description <String>]
 [-TargetPool <String[]>] [-PortName <String[]>] [-PortNumber <Int32[]>] [-NamedPort <NamedPort[]>]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -BaseInstanceName


```yaml
Type: System.String
Parameter Sets: ByZoneProperties, ByRegionProperties
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description


```yaml
Type: System.String
Parameter Sets: ByZoneProperties, ByRegionProperties
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstanceTemplate


```yaml
Type: System.String
Parameter Sets: ByZoneProperties, ByRegionProperties
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
Parameter Sets: ByZoneProperties, ByRegionProperties
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NamedPort


```yaml
Type: Google.Apis.Compute.v1.Data.NamedPort[]
Parameter Sets: ByZoneProperties, ByRegionProperties
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Object


```yaml
Type: Google.Apis.Compute.v1.Data.InstanceGroupManager
Parameter Sets: ByObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PortName


```yaml
Type: System.String[]
Parameter Sets: ByZoneProperties, ByRegionProperties
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PortNumber


```yaml
Type: System.Int32[]
Parameter Sets: ByZoneProperties, ByRegionProperties
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

### -Region


```yaml
Type: System.String
Parameter Sets: ByObject, ByRegionProperties
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetPool


```yaml
Type: System.String[]
Parameter Sets: ByZoneProperties, ByRegionProperties
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetSize


```yaml
Type: System.Int32
Parameter Sets: ByZoneProperties, ByRegionProperties
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Zone


```yaml
Type: System.String
Parameter Sets: ByZoneProperties, ByObject
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

### Google.Apis.Compute.v1.Data.InstanceGroupManager

## OUTPUTS

### Google.Apis.Compute.v1.Data.InstanceGroupManager

## NOTES

## RELATED LINKS
