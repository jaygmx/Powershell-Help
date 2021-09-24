---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# ConvertTo-MacOs9LineEnding

## SYNOPSIS
PSCX Cmdlet: Converts the line endings in the specified file to Mac OS9 and earlier style line endings "\r".

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
ConvertTo-MacOs9LineEnding [-Path] <String[]> [-Destination] <String> [-Force] [-NoClobber]
 [[-Encoding] <StringEncodingParameter>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
ConvertTo-MacOs9LineEnding [-LiteralPath] <String[]> [-Destination] <String> [-Force] [-NoClobber]
 [[-Encoding] <StringEncodingParameter>] [<CommonParameters>]
```

## DESCRIPTION
Converts the line endings in the specified file to Mac OS9 and earlier style line endings "\r". 
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
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

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
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### -Destination
Destination to write the converted file.
If the destination is a directory, then the file is written to the directory using the same name.

```yaml
Type: String
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
Type: SwitchParameter
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
Type: SwitchParameter
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
Type: StringEncodingParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS

[ConvertTo-UnixLineEnding]()

[ConvertTo-WindowsLineEnding]()

