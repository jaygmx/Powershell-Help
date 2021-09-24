---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/tricks/filesystem/finding-duplicate-files
schema: 2.0.0
---

# Find-PSOneDuplicateFile

## SYNOPSIS
Identifies files with duplicate content

## SYNTAX

```
Find-PSOneDuplicateFile [-Path] <String> [[-Filter] <String>] [<CommonParameters>]
```

## DESCRIPTION
Returns a hashtable with the hashes that have at least two files (duplicates)

## EXAMPLES

### EXAMPLE 1
```
$Path = [Environment]::GetFolderPath('MyDocuments')
Find-PSOneDuplicateFile -Path $Path 
Find duplicate files in the user documents folder
```

### EXAMPLE 2
```
Find-PSOneDuplicateFile -Path c:\windows -Filter *.log 
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one/tricks/filesystem/finding-duplicate-files](https://powershell.one/tricks/filesystem/finding-duplicate-files)

