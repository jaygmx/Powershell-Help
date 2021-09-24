---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Write-GcsObject

## SYNOPSIS


## SYNTAX

### ByObjectFromString
```
Write-GcsObject [-InputObject] <Object> [-Value <String>] [-ContentType <String>] [-ContentEncoding <String>]
 [-ContentLanguage <String>] [-ContentDisposition <String>] [-CacheControl <String>] [-Metadata <Hashtable>]
 [-Force] [<CommonParameters>]
```

### ByObjectFromFile
```
Write-GcsObject [-InputObject] <Object> -File <String> [-ContentType <String>] [-ContentEncoding <String>]
 [-ContentLanguage <String>] [-ContentDisposition <String>] [-CacheControl <String>] [-Metadata <Hashtable>]
 [-Force] [<CommonParameters>]
```

### ByNameFromString
```
Write-GcsObject [[-Bucket] <String>] [-ObjectName] <String> [-Value <String>] [-ContentType <String>]
 [-ContentEncoding <String>] [-ContentLanguage <String>] [-ContentDisposition <String>]
 [-CacheControl <String>] [-Metadata <Hashtable>] [-Force] [<CommonParameters>]
```

### ByNameFromFile
```
Write-GcsObject [[-Bucket] <String>] [-ObjectName] <String> -File <String> [-ContentType <String>]
 [-ContentEncoding <String>] [-ContentLanguage <String>] [-ContentDisposition <String>]
 [-CacheControl <String>] [-Metadata <Hashtable>] [-Force] [<CommonParameters>]
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
Parameter Sets: ByNameFromString, ByNameFromFile
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CacheControl


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

### -ContentDisposition


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

### -ContentEncoding


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

### -ContentLanguage


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

### -ContentType


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

### -File


```yaml
Type: System.String
Parameter Sets: ByObjectFromFile, ByNameFromFile
Aliases:

Required: True
Position: Named
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
Parameter Sets: ByObjectFromString, ByObjectFromFile
Aliases: Object

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Metadata


```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectName


```yaml
Type: System.String
Parameter Sets: ByNameFromString, ByNameFromFile
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value


```yaml
Type: System.String
Parameter Sets: ByObjectFromString
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.String
Parameter Sets: ByNameFromString
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

### Google.Apis.Storage.v1.Data.Object

### System.String

## OUTPUTS

### Google.Apis.Storage.v1.Data.Object

## NOTES

## RELATED LINKS
