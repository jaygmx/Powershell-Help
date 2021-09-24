---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# New-GcsObject

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### ContentsFromString (Default)
```
New-GcsObject [[-Bucket] <String>] [-ObjectName] <String> [[-Value] <String>] [-ContentType <String>]
 [-ContentEncoding <String>] [-ContentLanguage <String>] [-ContentDisposition <String>]
 [-CacheControl <String>] [-PredefinedAcl <PredefinedAclEnum>] [-Metadata <Hashtable>] [-Force]
 [<CommonParameters>]
```

### ContentsFromFile
```
New-GcsObject [[-Bucket] <String>] [[-ObjectName] <String>] [-File] <String> [-ContentType <String>]
 [-ContentEncoding <String>] [-ContentLanguage <String>] [-ContentDisposition <String>]
 [-CacheControl <String>] [-PredefinedAcl <PredefinedAclEnum>] [-Metadata <Hashtable>] [-Force]
 [<CommonParameters>]
```

### UploadFolder
```
New-GcsObject [[-Bucket] <String>] [-Folder] <String> [-ObjectNamePrefix <String>] [-ContentEncoding <String>]
 [-ContentLanguage <String>] [-ContentDisposition <String>] [-CacheControl <String>]
 [-PredefinedAcl <PredefinedAclEnum>] [-Metadata <Hashtable>] [-Force] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Bucket
{{ Fill Bucket Description }}

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
Parameter Sets: ContentsFromString, ContentsFromFile
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
Parameter Sets: ContentsFromFile
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Folder
{{ Fill Folder Description }}

```yaml
Type: System.String
Parameter Sets: UploadFolder
Aliases:

Required: True
Position: 2
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
Parameter Sets: ContentsFromString
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.String
Parameter Sets: ContentsFromFile
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectNamePrefix
{{ Fill ObjectNamePrefix Description }}

```yaml
Type: System.String
Parameter Sets: UploadFolder
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PredefinedAcl
{{ Fill PredefinedAcl Description }}

```yaml
Type: System.Nullable`1[Google.Apis.Storage.v1.ObjectsResource+InsertMediaUpload+PredefinedAclEnum]
Parameter Sets: (All)
Aliases:
Accepted values: AuthenticatedRead, BucketOwnerFullControl, BucketOwnerRead, Private__, ProjectPrivate, PublicRead

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value
{{ Fill Value Description }}

```yaml
Type: System.String
Parameter Sets: ContentsFromString
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Google.Apis.Storage.v1.Data.Object

## NOTES

## RELATED LINKS
