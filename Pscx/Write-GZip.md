---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Write-GZip

## SYNOPSIS
PSCX Cmdlet: Create GNU ZIP (GZIP) format files from pipeline or parameter input.

## SYNTAX

### Path (Default)
```
Write-GZip [-Level <Int32>] [[-OutputPath] <PscxPathInfo>] [-NoClobber] [-Quiet] [-Path] <PscxPathInfo[]>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### LiteralPath
```
Write-GZip [-Level <Int32>] [[-OutputPath] <PscxPathInfo>] [-NoClobber] [-Quiet]
 [-LiteralPath] <PscxPathInfo[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Object
```
Write-GZip [-Level <Int32>] [[-OutputPath] <PscxPathInfo>] [[-EntryPathRoot] <PscxPathInfo>] [-NoClobber]
 [-Quiet] -InputObject <PSObject> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create GNU ZIP (GZIP) format files from pipeline or parameter input.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
PS> dir c:\logs\ -rec -inc *.log | write-tar -output logs.tar | write-gzip -level 9 | move-item c:\archived_logs\
```

This will recursively search C:\logs for *.log files, archive them into a single tar, compress the resulting tar with gzip and move it to c:\archived_logs.

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

### -EntryPathRoot
@{Text=}

```yaml
Type: Pscx.IO.PscxPathInfo
Parameter Sets: Object
Aliases: Root

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
Type: Pscx.IO.PscxPathInfo
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: Not set.
Accept pipeline input: False
Accept wildcard characters: False
```

### -Level
Can be set between 1 and 9 inclusive.
Higher numbers use a more efficient compression method, resulting in smaller archives.
Higher levels generally result in slower compression times.

```yaml
Type: System.Nullable`1[System.Int32]
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
Type: System.Management.Automation.SwitchParameter
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

## OUTPUTS

## NOTES

## RELATED LINKS
