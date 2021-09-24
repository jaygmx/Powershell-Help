---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one
schema: 2.0.0
---

# Find-PSOneDuplicateFileFast

## SYNOPSIS
Identifies files with duplicate content and uses a partial hash for large files to speed calculation up

## SYNTAX

```
Find-PSOneDuplicateFileFast [-Path] <String> [[-Filter] <String>] [-TestPartialHash] [[-MaxFileSize] <Int64>]
 [<CommonParameters>]
```

## DESCRIPTION
Returns a hashtable with the hashes that have at least two files (duplicates).
Large files with partial hashes are suffixed with a "P".
Large files with a partial hash can be falsely positive: they may in fact be different even though the partial hash is the same
You either need to calculate the full hash for these files to be absolutely sure, or add -TestPartialHash.
Calculating a full hash for large files may take a very long time though.
So you may be better off using other
strategies to identify duplicate file content, i.e.
look at identical creation times, etc.

## EXAMPLES

### EXAMPLE 1
```
$Path = [Environment]::GetFolderPath('MyDocuments')
Find-PSOneDuplicateFileFast -Path $Path 
Find duplicate files in the user documents folder
```

### EXAMPLE 2
```
Find-PSOneDuplicateFileFast -Path c:\windows -Filter *.log 
find log files in the Windows folder with duplicate content
```

## PARAMETERS

### -Path
Path of folder to recursively search

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

### -Filter
Filter to apply.
Default is '*' (all Files)

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: *
Accept pipeline input: False
Accept wildcard characters: False
```

### -TestPartialHash
when there are multiple files with same partial hash
they may still be different.
When setting this switch,
full hashes are calculated which may take a very long time
for large files and/or slow networks

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxFileSize
use partial hashes for files larger than this:

```yaml
Type: System.Int64
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 102400
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one](https://powershell.one)

