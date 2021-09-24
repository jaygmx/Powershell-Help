---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Write-Zip

## SYNOPSIS
PSCX Cmdlet: Create ZIP format archive files from pipline or parameter input.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Write-Zip [-LiteralPath] <String[]> [[-OutputPath] <String>] [-Append] [-FlattenPaths]
 [-IncludeEmptyDirectories] [-Level <Nullable`1>] [-NoClobber] [-Quiet] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Write-Zip -InputObject <PSObject> [[-EntryPathRoot] <String>] [-Append] [-FlattenPaths]
 [-IncludeEmptyDirectories] [-Level <Nullable`1>] [-NoClobber] [-Quiet] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Write-Zip [-Path] <String[]> [-Append] [-FlattenPaths] [-IncludeEmptyDirectories] [-Level <Nullable`1>]
 [-NoClobber] [-Quiet] [<CommonParameters>]
```

## DESCRIPTION
Create ZIP format archive files from pipline or parameter input.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
PS> write-zip .\Desktop desktop.zip
```

This will zip the contents of the Desktop directory into the file desktop.zip.

### EXAMPLE 2
PS C:\\\>

```
PS> dir c:\logs\ -rec -inc *.log | write-zip -level 9 | move-item c:\archived_logs\
```

This will recursively search C:\logs for *.log files, compress them with maximum compression, move them to c:\archived_logs.

## PARAMETERS

### -LiteralPath
Specifies a path to the item.
The value of -LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell Windows PowerShell not to interpret any characters as escape sequences.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: N/A
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Specifies the path to the file to process.
Wildcard syntax is allowed.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: True
Position: 1
Default value: N/A
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InputObject
Accepts an object as input to the cmdlet.
Enter a variable that contains the objects or type a command or expression that gets the objects.

```yaml
Type: PSObject
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: Named
Default value: N/A
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -EntryPathRoot
@{Text=}

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputPath
If set, a single archive will be created with all input files stored in it.
If not set, each archive will be stored in a separate archive in the current directory.
This must be set to an output filename, not a directory.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: 2
Default value: Not set.
Accept pipeline input: False
Accept wildcard characters: False
```

### -Append
If set, the input files will be added to, or updated in, the zip file specified by OutputPath.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FlattenPaths
If set, no path information will be stored in the archive, effectively placing all files in the root.
Files in subdirectories matching those in lower levels with clashing names will not be added and a warning will be emitted.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Not set.
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeEmptyDirectories
If set, empty directories will be added as entries into the archive.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Not set.
Accept pipeline input: False
Accept wildcard characters: False
```

### -Level
Can be set between 1 and 9 inclusive.
Higher numbers use a more efficient compression method, resulting in smaller archives.
Higher levels generally result in slower compression times.

```yaml
Type: Nullable`1
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 5
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoClobber
If set, existing archives with the same name as the current output archive will not be overwritten.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Not set, existing archives with the same name WILL be overwritten.
Accept pipeline input: False
Accept wildcard characters: False
```

### -Quiet
@{Text=}

```yaml
Type: SwitchParameter
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

## OUTPUTS

## NOTES
* When passing DirectoryInfo objects via the pipeline, the Cmdlet will NOT iterate their contents. However, if you pass a directory name via -Path, they WILL be iterated for contents.

## RELATED LINKS
