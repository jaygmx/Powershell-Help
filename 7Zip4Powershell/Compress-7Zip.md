---
external help file: 7Zip4PowerShell.dll-Help.xml
Module Name: 7Zip4Powershell
online version:
schema: 2.0.0
---

# Compress-7Zip

## SYNOPSIS


## SYNTAX

### NoPassword (Default)
```
Compress-7Zip [-ArchiveFileName] <String> [-Path] <String> [[-Filter] <String>] [-OutputPath <String>]
 [-Format <OutputFormat>] [-CompressionLevel <CompressionLevel>] [-CompressionMethod <CompressionMethod>]
 [-CustomInitialization <ScriptBlock>] [-EncryptFilenames] [-FlattenDirectoryStructure] [-VolumeSize <Int64>]
 [-SkipEmptyDirectories] [-PreserveDirectoryRoot] [-DisableRecursion] [-Append] [<CommonParameters>]
```

### PlainPassword
```
Compress-7Zip [-ArchiveFileName] <String> [-Path] <String> [[-Filter] <String>] [-OutputPath <String>]
 [-Format <OutputFormat>] [-CompressionLevel <CompressionLevel>] [-CompressionMethod <CompressionMethod>]
 [-Password <String>] [-CustomInitialization <ScriptBlock>] [-EncryptFilenames] [-FlattenDirectoryStructure]
 [-VolumeSize <Int64>] [-SkipEmptyDirectories] [-PreserveDirectoryRoot] [-DisableRecursion] [-Append]
 [<CommonParameters>]
```

### SecurePassword
```
Compress-7Zip [-ArchiveFileName] <String> [-Path] <String> [[-Filter] <String>] [-OutputPath <String>]
 [-Format <OutputFormat>] [-CompressionLevel <CompressionLevel>] [-CompressionMethod <CompressionMethod>]
 [-SecurePassword <SecureString>] [-CustomInitialization <ScriptBlock>] [-EncryptFilenames]
 [-FlattenDirectoryStructure] [-VolumeSize <Int64>] [-SkipEmptyDirectories] [-PreserveDirectoryRoot]
 [-DisableRecursion] [-Append] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Append
Append files to existing archive

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

### -CompressionLevel


```yaml
Type: SevenZip.CompressionLevel
Parameter Sets: (All)
Aliases:
Accepted values: None, Fast, Low, Normal, High, Ultra

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CompressionMethod


```yaml
Type: SevenZip.CompressionMethod
Parameter Sets: (All)
Aliases:
Accepted values: Copy, Deflate, Deflate64, BZip2, Lzma, Lzma2, Ppmd, Default

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomInitialization
Allows setting additional parameters on SevenZipCompressor

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

### -DisableRecursion
Disables recursive files search

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

### -EncryptFilenames
Enables encrypting filenames when using the 7z format

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

### -Filter
The filter to be applied if Path points to a directory

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FlattenDirectoryStructure
Disables preservation of directory structure

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

### -Format


```yaml
Type: SevenZip4PowerShell.OutputFormat
Parameter Sets: (All)
Aliases:
Accepted values: Auto, SevenZip, Zip, GZip, BZip2, Tar, XZ

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputPath
Output path for a compressed archive

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

### -Path
The source folder or file

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PreserveDirectoryRoot
Preserves directory root

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

### -SkipEmptyDirectories
Disables preservation of empty directories

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

### -VolumeSize
Specifies the volume sizes in bytes, 0 for no volumes

```yaml
Type: System.Int64
Parameter Sets: (All)
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

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
