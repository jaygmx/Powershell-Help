---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# Set-ReadOnly

## SYNOPSIS
Sets a file's read only status to true making it read only.

## SYNTAX

### Path (Default)
```
Set-ReadOnly [-Path] <String[]> [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### LiteralPath
```
Set-ReadOnly [-LiteralPath] <String[]> [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Sets a file's read only status to true making it read only.

## EXAMPLES

### EXAMPLE 1
```
Set-ReadOnly foo.txt
Makes foo.txt read only.
```

### EXAMPLE 2
```
Set-ReadOnly [a-h]*.txt -passthru
Makes any .txt file start with the letters a thru h read only and passes the filenames down the pipeline.
```

### EXAMPLE 3
```
Get-ChildItem bar[0-9].txt | Set-ReadOnly
Set-ReadOnly can accept pipeline input corresponding to files and make them all read only.
```

## PARAMETERS

### -Path
The path to the file make read only. 
Wildcards are accepted.

```yaml
Type: System.String[]
Parameter Sets: Path
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LiteralPath
Specifies the path to a file make read only.
Unlike Path, the value of LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in
single quotation marks.
Single quotation marks tell Windows PowerShell not to interpret any characters
as escape sequences.

```yaml
Type: System.String[]
Parameter Sets: LiteralPath
Aliases: PSPath

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Passes the pipeline input object down the pipeline.
By default, this cmdlet does not generate any output.

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
