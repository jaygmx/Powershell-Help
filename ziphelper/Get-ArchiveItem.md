---
external help file: ziphelper-help.xml
Module Name: ziphelper
online version:
schema: 2.0.0
---

# Get-ArchiveItem

## SYNOPSIS
Returns archive items from the archive file

## SYNTAX

```
Get-ArchiveItem [-Path] <String> [[-Item] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Returns a list of archive files from the archive.
Returns item contents as a byte array when specific items are provided.

## EXAMPLES

### EXAMPLE 1
```
# Return an archive file list
Get-ArchiveItem .\asd.zip
```

### EXAMPLE 2
```
# Return an archive file with binary contents
Get-ArchiveItem .\asd.zip asd\file1.txt
```

## PARAMETERS

### -Path
Archive Path

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

### -Item
Path to existing items inside the archive

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
General notes

## RELATED LINKS
