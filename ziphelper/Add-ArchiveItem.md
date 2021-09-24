---
external help file: ziphelper-help.xml
Module Name: ziphelper
online version:
schema: 2.0.0
---

# Add-ArchiveItem

## SYNOPSIS
Adds one or more items to the archive

## SYNTAX

```
Add-ArchiveItem [-Path] <String> [-Item] <String[]> [-InnerFolder <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Adds specific file or folder to the existing archive

## EXAMPLES

### EXAMPLE 1
```
# Put two txt files into archive.zip\inner_folder\path\
Add-ArchiveItem -Path c:\temp\myarchive.zip -Item MyFile.txt, Myfile2.txt -InnerFolder inner_folder\path
```

## PARAMETERS

### -Path
Archive path

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Item
Archived item: file or folder

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InnerFolder
\[switch\]$Force,
\[switch\]$Recurse

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: .
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
