---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Copy-GcsObject

## SYNOPSIS


## SYNTAX

### ByObject (Default)
```
Copy-GcsObject -InputObject <Object> [[-DestinationBucket] <String>] [[-DestinationObjectName] <String>]
 [-Force] [<CommonParameters>]
```

### ByName
```
Copy-GcsObject [-Bucket <String>] -ObjectName <String> [[-DestinationBucket] <String>]
 [[-DestinationObjectName] <String>] [-Force] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Bucket


```yaml
Type: System.String
Parameter Sets: ByName
Aliases: SourceBucket

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestinationBucket


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestinationObjectName


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force


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

### -InputObject


```yaml
Type: Google.Apis.Storage.v1.Data.Object
Parameter Sets: ByObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ObjectName


```yaml
Type: System.String
Parameter Sets: ByName
Aliases: SourceObjectName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Google.Apis.Storage.v1.Data.Object

## OUTPUTS

### Google.Apis.Storage.v1.Data.Object

## NOTES

## RELATED LINKS
