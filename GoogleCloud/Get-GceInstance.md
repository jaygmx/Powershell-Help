---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Get-GceInstance

## SYNOPSIS


## SYNTAX

### OfProject (Default)
```
Get-GceInstance [-Project <String>] [-SerialPortOutput] [-PortNumber <Int32>] [<CommonParameters>]
```

### OfZone
```
Get-GceInstance [-Project <String>] -Zone <String> [-SerialPortOutput] [-PortNumber <Int32>]
 [<CommonParameters>]
```

### ByName
```
Get-GceInstance [-Project <String>] [-Zone <String>] [-Name] <String> [-SerialPortOutput] [-PortNumber <Int32>]
 [<CommonParameters>]
```

### OfInstanceGroupManager
```
Get-GceInstance [-Project <String>] [-Zone <String>] -ManagedGroupName <String> [-SerialPortOutput]
 [-PortNumber <Int32>] [<CommonParameters>]
```

### ByObject
```
Get-GceInstance [-Object] <Instance> [-SerialPortOutput] [-PortNumber <Int32>] [<CommonParameters>]
```

### OfInstanceGroupManagerObject
```
Get-GceInstance [-ManagedGroupObject] <InstanceGroupManager> [-SerialPortOutput] [-PortNumber <Int32>]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -ManagedGroupName


```yaml
Type: System.String
Parameter Sets: OfInstanceGroupManager
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManagedGroupObject


```yaml
Type: Google.Apis.Compute.v1.Data.InstanceGroupManager
Parameter Sets: OfInstanceGroupManagerObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name


```yaml
Type: System.String
Parameter Sets: ByName
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Object


```yaml
Type: Google.Apis.Compute.v1.Data.Instance
Parameter Sets: ByObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PortNumber


```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
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
Parameter Sets: OfProject, OfZone, ByName, OfInstanceGroupManager
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SerialPortOutput


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Zone


```yaml
Type: System.String
Parameter Sets: OfZone
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.String
Parameter Sets: ByName, OfInstanceGroupManager
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

### System.String

### Google.Apis.Compute.v1.Data.Instance

### Google.Apis.Compute.v1.Data.InstanceGroupManager

## OUTPUTS

### Google.Apis.Compute.v1.Data.Instance

### System.String

## NOTES

## RELATED LINKS
