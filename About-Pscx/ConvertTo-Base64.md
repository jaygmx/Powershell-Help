---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# ConvertTo-Base64

## SYNOPSIS
PSCX Cmdlet: Converts byte array or specified file contents to base64 string.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
ConvertTo-Base64 [-Path] <String[]> [-NoLineBreak] [-Stream] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
ConvertTo-Base64 -InputObject <PSObject> [-NoLineBreak] [-Stream] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
ConvertTo-Base64 [-LiteralPath] <String[]> [-NoLineBreak] [-Stream] [<CommonParameters>]
```

## DESCRIPTION
Converts byte array or specified file contents to base64 string. 
By default, this cmdlet inserts line breaks every 76 characters and outputs the result in a single string.
For very large files, you may run into OutOfMemoryExceptions.
In this case, use the -Stream parameter which will generate multiple string outputs that, combined together, result in the equivalent base 64 text.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
[byte[]](1..127) | ConvertTo-Base64
```

This buffers up the steam of bytes and then outputs the base64 string.

### EXAMPLE 2
PS C:\\\>

```
$arr = [byte[]](1..127); ConvertTo-Base64 -Inp $arr
```

This outputs the base64 string based on the byte array passed into the InputObject parameter.

### EXAMPLE 3
PS C:\\\>

```
$b64 = ConvertTo-Base64 Foo.dll -NoLineBreak
```

Converts the specified file (read as binary) to a base 64 string.

### EXAMPLE 4
PS C:\\\>

```
ConvertTo-Base64 $PSHome\PowerShell.exe -stream > b64.txt
```

When dealing with large files it is usually better to pass the path to ConvertTo-Base64.

## PARAMETERS

### -LiteralPath
@{Text=}

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
@{Text=}

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InputObject
@{Text=}

```yaml
Type: PSObject
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NoLineBreak
Suppress line breaks that are added by default every 76 characters.

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

### -Stream
Outputs multiple strings for the base 64 encoded data.
By default, the bytes are accumulated and encoded as a single string which can generate OutOfMemoryExceptions for very large files.

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

## RELATED LINKS

[ConvertFrom-Base64]()

