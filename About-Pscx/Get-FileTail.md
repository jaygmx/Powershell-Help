---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Get-FileTail

## SYNOPSIS
PSCX Cmdlet: Tails the contents of a file - optionally waiting on new content.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-FileTail [-Path] <String[]> [-Count <Int32>] [-Encoding <EncodingParameter>] [-LineTerminator <String>]
 [-Wait] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-FileTail [-LiteralPath] <String[]> [-Count <Int32>] [-Encoding <EncodingParameter>]
 [-LineTerminator <String>] [-Wait] [<CommonParameters>]
```

## DESCRIPTION
This implentation efficiently tails the contents of a file by reading lines from the end rather then processing the entire file.
This behavior is crucial for efficiently tailing large log files and large log files over a network. 
You can also specify the Wait parameter to have the cmdlet wait and display new content as it is written to the file. 
Use Ctrl+C to break out of the wait loop. 
Note that if an encoding is not specified, the cmdlet will attempt to auto-detect the encoding by reading the first character from the file.
If no character haven't been written to the file yet, the cmdlet will default to using Unicode encoding.
You can override this behavior by explicitly specifying the encoding via the Encoding parameter.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\> Tail-File foo.log -Count 20
```

Displays the last 20 lines of the file foo.log. 
If there are fewer than 20 lines, it will display all lines.

### EXAMPLE 1
PS C:\\\>

```
C:\> Tail-File ascii.log -Wait -Encoding Ascii
```

Displays the last 10 lines of the ASCII encoded file ascii.log and then waits. 
Any new content appended to the file will be displayed. 
Press Ctrl+C to break out of the loop and return control to the console.

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

### -Count
The number of lines to display from the end of the file.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 10
Accept pipeline input: False
Accept wildcard characters: False
```

### -Encoding
The encoding to use for string InputObjects. 
Valid values are: ASCII, Unicode and UTF8.
If the file contains only ASCII characters specify the parameter "-Encoding ASCII" on the file.
UTF8 is only supported if the file contains ASCII characters.

```yaml
Type: EncodingParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Unicode (if the encoding cannot be detected by reading the first 1 character from the file)
Accept pipeline input: False
Accept wildcard characters: False
```

### -LineTerminator
The line termination sequence for the file.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: [System.Environment]::NewLine
Accept pipeline input: False
Accept wildcard characters: False
```

### -Wait
Puts Tail-File into an infinite wait loop, waiting for new content to be appended to the file. 
When new content is appended to the file it will be displayed. 
Use Ctrl+C to exit the wait loop.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
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
