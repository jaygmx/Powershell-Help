---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Format-PscxHex

## SYNOPSIS
PSCX Cmdlet: Displays the contents of files or byte streams in hex format and optionally ASCII.

## SYNTAX

### Path (Default)
```
Format-PscxHex [-Width <Int32>] [-Columns <Int32>] [-Offset <Int64>] [-Count <Int32>] [-HideHeader]
 [-HideAddress] [-HideAscii] [-Path] <PscxPathInfo[]> [<CommonParameters>]
```

### Object
```
Format-PscxHex [-Width <Int32>] [-Columns <Int32>] [-Offset <Int64>] [-Count <Int32>] [-HideHeader]
 [-HideAddress] [-HideAscii] [-StringEncoding <StringEncodingParameter>] -InputObject <PSObject>
 [<CommonParameters>]
```

### LiteralPath
```
Format-PscxHex [-Width <Int32>] [-Columns <Int32>] [-Offset <Int64>] [-Count <Int32>] [-HideHeader]
 [-HideAddress] [-HideAscii] [-LiteralPath] <PscxPathInfo[]> [<CommonParameters>]
```

## DESCRIPTION
The Format-PscxHex command displays the contents of the specified files in hex format. 
This cmdlet will also accept pipeline input in the form of a byte stream. 
The output can be controlled via various parameters to indicate the number of columns that should be displayed or alternatively you can specify the width of the output. 
The header, address and ASCII portions of the display can also be turned off individually. 
The offset and count can also be specified via parameters to control where in the input to start displaying and how much to display.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\PS>Format-PscxHex $pshome\PowerShell.exe -Count 256
```

This displays the first 256 bytes of the PowerShell executable.

### EXAMPLE 2
PS C:\\\>

```
C:\PS>[byte[]](1..255) | Format-PscxHex
```

This examples accepts a byte array as input and displays those byte values in hex and ASCII.

### EXAMPLE 3
PS C:\\\>

```
C:\PS>"hello world" | Format-PscxHex -InputObject {$_}
```

In this scenario the string is always converted to bytes assuming the string encoding is Unicode which is true of PowerShell strings.

### EXAMPLE 4
PS C:\\\>

```
C:\PS>"hello world" | Format-PscxHex -InputObject {$_} -StringEncoding ASCII
```

If you want to view the bytes using an alternate encoding then use the -StringEncoding parameter to specify the preferred encoding.

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

### -Columns
@{Text=}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases: NumBytesPerLine

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Count
Specifies the number of bytes to display.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HideAddress
Hides the address information.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: NoAddress

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HideAscii
Hides the ASCII representation of the bytes.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: NoAscii

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HideHeader
Hides the header lines.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: NoHeader

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Offset
Specifies the number of bytes to offset into file.

```yaml
Type: System.Int64
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StringEncoding
The encoding to use for string InputObjects. 
Valid values are: ASCII, UTF7, UTF8, UTF32, Unicode, BigEndianUnicode and Default.

```yaml
Type: Pscx.StringEncodingParameter
Parameter Sets: Object
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Width
Specifies desired width of output text.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### byte
### byte[]
### string
## OUTPUTS

### Formatted text
## NOTES
Strings can be viewed in hex but because the cmdlet interprets pipeline input of type string to specify a file path you need to use the -InputObject parameter. 
See example number three below.

## RELATED LINKS
