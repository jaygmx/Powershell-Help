---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloudBeta
online version:
schema: 2.0.0
---

# Get-GkeNodePool

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ByClusterName
```
Get-GkeNodePool [-Project <String>] [-Zone <String>] [-ClusterName] <String> [[-NodePoolName] <String[]>]
 [<CommonParameters>]
```

### ByClusterObject
```
Get-GkeNodePool [[-NodePoolName] <String[]>] [-ClusterObject] <Cluster> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -ClusterName
{{ Fill ClusterName Description }}

```yaml
Type: System.String
Parameter Sets: ByClusterName
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClusterObject
{{ Fill ClusterObject Description }}

```yaml
Type: Google.Apis.Container.v1.Data.Cluster
Parameter Sets: ByClusterObject
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NodePoolName
{{ Fill NodePoolName Description }}

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

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
Parameter Sets: ByClusterName
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
Parameter Sets: ByClusterName
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

### Google.Apis.Container.v1.Data.Cluster

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
