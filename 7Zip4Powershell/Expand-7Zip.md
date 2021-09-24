---
external help file: 7Zip4PowerShell.dll-Help.xml
Module Name: 7Zip4Powershell
online version:
schema: 2.0.0
---

# Expand-7Zip

## SYNOPSIS


## SYNTAX

### NoPassword (Default)
```
Expand-7Zip [-ArchiveFileName] <String> [-TargetPath] <String> [-CustomInitialization <ScriptBlock>]
 [<CommonParameters>]
```

### PlainPassword
```
Expand-7Zip [-ArchiveFileName] <String> [-TargetPath] <String> [-Password <String>]
 [-CustomInitialization <ScriptBlock>] [<CommonParameters>]
```

### SecurePassword
```
Expand-7Zip [-ArchiveFileName] <String> [-TargetPath] <String> [-SecurePassword <SecureString>]
 [-CustomInitialization <ScriptBlock>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -ArchiveFileName
The full file name of the archive

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomInitialization
Allows setting additional parameters on SevenZipExtractor

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Password


```yaml
Type: System.String
Parameter Sets: PlainPassword
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SecurePassword


```yaml
Type: System.Security.SecureString
Parameter Sets: SecurePassword
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetPath
The target folder

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
