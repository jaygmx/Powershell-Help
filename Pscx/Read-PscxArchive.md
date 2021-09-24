---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Read-PscxArchive

## SYNOPSIS
PSCX Cmdlet: Enumerates compressed archives such as 7z or rar, emitting ArchiveEntry objects representing records in the archive.

## SYNTAX

### Path (Default)
```
Read-PscxArchive [-ShowProgress] [-IncludeDirectories] [-Path] <PscxPathInfo[]> [<CommonParameters>]
```

### Object
```
Read-PscxArchive [-ShowProgress] [-IncludeDirectories] -InputObject <PSObject> [<CommonParameters>]
```

### LiteralPath
```
Read-PscxArchive [-ShowProgress] [-IncludeDirectories] [-LiteralPath] <PscxPathInfo[]> [<CommonParameters>]
```

## DESCRIPTION
Enumerates compressed archives such as 7z or rar, emitting ArchiveEntry objects representing records in the archive.Read-PscxArchive is used to list the contents of a compressed archive containing one or more compressed file(s).
The format of the file being read can be overriden with the Format parameter, for example to enumerate the contents of a self-extracting archive (EXE).Read-PscxArchive is useful if you wish to perform filtering using standard pipeline Where-Object and/or ForEach-Object cmdlets before piping ArchiveEntry objects to Expand-PscxArchive.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
Read-PscxArchive -Path *.iso > contents.txt
```

Read all ISO compressed archives and dump the contents into a text file.

### EXAMPLE 2
PS C:\\\>

```
Read-PscxArchive -Path Setup.exe -Format Zip | Where-Object { $_.Name -like "*.txt" } | Expand-PscxArchive
```

Read contents from a self-extracting zip file and expand any txt files into the current filesystem location.

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

### -IncludeDirectories
If present, directs Read-PscxArchive to list the 0-length directory entries that represent folders in the archive.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.IO.FileInfo
## OUTPUTS

### Pscx.IO.Compression.ArchiveEntry
## NOTES
Supported formats are: SevenZip, Arj, BZip2, Cab, Chm, Compound, Cpio, Deb, GZip, Iso, Lzh, Lzma, Nsis, Rar, Rpm, Split, Tar, Wim, Z, Zip.

## RELATED LINKS
