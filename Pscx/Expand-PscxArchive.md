---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Expand-PscxArchive

## SYNOPSIS
PSCX Cmdlet: Expands a compressed archive file, or ArchiveEntry object, to its constituent file(s).

## SYNTAX

### Path (Default)
```
Expand-PscxArchive [-Index <Int32[]>] [-EntryPath <String[]>] [[-OutputPath] <PscxPathInfo>]
 [-Password <SecureString>] [-FlattenPaths] [-PassThru] [-ShowProgress] [-Force] [-Path] <PscxPathInfo[]>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Object
```
Expand-PscxArchive [-Index <Int32[]>] [-EntryPath <String[]>] [[-OutputPath] <PscxPathInfo>]
 [-Password <SecureString>] [-FlattenPaths] [-PassThru] [-ShowProgress] [-Force] -InputObject <PSObject>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### LiteralPath
```
Expand-PscxArchive [-Index <Int32[]>] [-EntryPath <String[]>] [[-OutputPath] <PscxPathInfo>]
 [-Password <SecureString>] [-FlattenPaths] [-PassThru] [-ShowProgress] [-Force]
 [-LiteralPath] <PscxPathInfo[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Expands a compressed archive file, or ArchiveEntry object, to its constituent file(s).

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
Expand-PscxArchive -Path *.zip -OutputPath .\Temp\ -ShowProgress
```

Expand all zip files in the current directory to .\temp while showing a progress bar.

### EXAMPLE 2
PS C:\\\>

```
Expand-PscxArchive -Path setup.exe -EntryPath en-us\readme.htm
```

Search a self-expanding zip file named setup.exe in the current directory for a file named "readme.htm" in a subdirectory named "en-us," and expand it to the current directory.

### EXAMPLE 3
PS C:\\\>

```
Read-PscxArchive *.iso | where { $_.size -gt 1mb } | Expand-PscxArchive
```

Scan through all ISOs in the current directory and expand any files bigger than 1MB to the current directory.

### EXAMPLE 4
PS C:\\\>

```
dir x:\ISOs -rec -inc *.iso | Read-PscxArchive | where {$_.path -eq "setup.exe"} | extract-PscxArchive -path {$_.archivepath} -index (0..19)
```

Look through all files under x:\ISOs for ISOs that contain a setup.exe in the root, and if so, expand the first twenty files of that ISO to the current directory.

## PARAMETERS

### -LiteralPath
Specifies a path to the item.
The value of -LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell Windows PowerShell not to interpret any characters as escape sequences.

```yaml
Type: Pscx.IO.PscxPathInfo[]
Parameter Sets: LiteralPath
Aliases: PSPath

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Specifies the path to the file to process.
Wildcard syntax is allowed.

```yaml
Type: Pscx.IO.PscxPathInfo[]
Parameter Sets: Path
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InputObject
Accepts an object as input to the cmdlet.
Enter a variable that contains the objects or type a command or expression that gets the objects.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: Object
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OutputPath
The path to place the expanded file(s).
This path must lie on the FileSystem provider.

```yaml
Type: Pscx.IO.PscxPathInfo
Parameter Sets: (All)
Aliases: To

Required: False
Position: 1
Default value: The current location of the FileSystem provider.
Accept pipeline input: False
Accept wildcard characters: False
```

### -EntryPath
The relative path of the file or file(s) inside the archive to expand.
For multiple files, use array syntax (comma-separated).

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FlattenPaths
Store all files in the archives in the root.
If multiple files have the same name, the last file in, wins.

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

### -Force
@{Text=}

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

### -Index
The index, or indices, of the file(s) inside the archive to expand.
For multiple indices, use array syntax (comma-separated).

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Output a FileInfo or DirectoryInfo for each file or directory expanded, respectively.

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

### -Password
A password to decrypt encrypted entries in the archive, if required.

```yaml
Type: System.Security.SecureString
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Not Set
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShowProgress
Show the PowerShell progress bar while performing expansion and scanning operations.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.IO.FileInfo
### Pscx.IO.Compression.ArchiveEntry
## OUTPUTS

### System.IO.FileSystemInfo
## NOTES
Supported formats are: SevenZip, Arj, BZip2, Cab, Chm, Compound, Cpio, Deb, GZip, Iso, Lzh, Lzma, Nsis, Rar, Rpm, Split, Tar, Wim, Z, Zip.

## RELATED LINKS
