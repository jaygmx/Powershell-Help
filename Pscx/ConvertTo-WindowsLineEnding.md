---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# ConvertTo-WindowsLineEnding

## SYNOPSIS
PSCX Cmdlet: Converts the line endings in the specified file to Windows line endings "\r\n".

## SYNTAX

### Path (Default)
```
ConvertTo-WindowsLineEnding [-Destination] <String> [[-Encoding] <StringEncodingParameter>] [-Force]
 [-NoClobber] [-Path] <PscxPathInfo[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### LiteralPath
```
ConvertTo-WindowsLineEnding [-Destination] <String> [[-Encoding] <StringEncodingParameter>] [-Force]
 [-NoClobber] [-LiteralPath] <PscxPathInfo[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Converts the line endings in the specified file to Windows line endings "\r\n". 
You can convert a single file to a new file name. 
Or you can convert multiple files and specify a destination directory. 
By default, this cmdlet will overwrite existing files unless you specify -NoClobber. 
If you want to force the overwrite of read only files use the -Force option.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

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
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Destination
Destination to write the converted file.
If the destination is a directory, then the file is written to the directory using the same name.

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

### -Force
Overwrite any existing readonly file.

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

### -NoClobber
Specifies not to overwrite any existing file.

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

### -Encoding
Encoding used to write the output file.
By default the encoding of the input file is used. 
Valid values are: unicode, utf7, utf8, utf32, ascii and bigendianunicode

```yaml
Type: Pscx.StringEncodingParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
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

[ConvertTo-MacOs9LineEnding]()

[ConvertTo-UnixLineEnding]()

