---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one
schema: 2.0.0
---

# Assert-PsOneFolderExists

## SYNOPSIS
Makes sure the specified folder(s) exist

## SYNTAX

```
Assert-PsOneFolderExists [-Path] <String[]> [<CommonParameters>]
```

## DESCRIPTION
If a folder does not exist, it will be created.

## EXAMPLES

### EXAMPLE 1
```
($Path = 'C:\test') | Assert-PsOneFolderExists
Makes sure the folder c:\test exists. If it is still missing, it will be created.
```

### EXAMPLE 2
```
'C:\test','c:\test2' | Assert-PsOneFolderExists
Makes sure the folders. If a folder is still missing, it will be created.
```

### EXAMPLE 3
```
Assert-PsOneFolderExists -Path 'C:\test','c:\test2'
Makes sure the folders. If a folder is still missing, it will be created.
```

## PARAMETERS

### -Path
Path to folder that must exist

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one](https://powershell.one)

