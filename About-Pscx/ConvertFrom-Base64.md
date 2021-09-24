---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# ConvertFrom-Base64

## SYNOPSIS
PSCX Cmdlet: Converts base64 encoded string to byte array.

## SYNTAX

```
ConvertFrom-Base64 [-Base64Text] <String[]> [-OutputPath <String>] [<CommonParameters>]
```

## DESCRIPTION
Converts base64 encoded string to byte array.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
$b64 | ConvertFrom-Base64 -OutputPath foo.dll
```

Converts the Base64 string in $b64 to a byte array and stores it in the foo.dll file.

### EXAMPLE 2
PS C:\\\>

```
ConvertFrom-Base64 -Base64Text $b64 -OutputPath foo.dll
```

Converts the Base64 string in $b64 to a byte array and stores it in the foo.dll file.

## PARAMETERS

### -Base64Text
Base64 encoded string to be converted into byte arary.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OutputPath
The path to write the results to. 
The results are written in binary format.

```yaml
Type: String
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

## OUTPUTS

## NOTES
* If an OutputPath is not specified then an array of bytes is output.  Using the OutputPath parameter is faster than using 'set-content -enc byte foo.dll' to write the output to a file.

## RELATED LINKS

[ConvertTo-Base64]()

