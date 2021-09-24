---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Write-GcsObject

## SYNOPSIS
{{ Fill in the Synopsis }}

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
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Bucket
{{ Fill Bucket Description }}

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
{{ Fill CacheControl Description }}

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
{{ Fill ContentDisposition Description }}

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
{{ Fill ContentEncoding Description }}

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
{{ Fill ContentLanguage Description }}

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
{{ Fill ContentType Description }}

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
{{ Fill File Description }}

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
{{ Fill Force Description }}

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
{{ Fill InputObject Description }}

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
{{ Fill Metadata Description }}

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
{{ Fill ObjectName Description }}

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
{{ Fill Value Description }}

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
