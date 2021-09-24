---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-Hash

## SYNOPSIS
PSCX Cmdlet: Gets the hash value for the specified file or byte array via the pipeline.

## SYNTAX

### Path (Default)
```
Get-Hash [-Algorithm <String>] [-Path] <PscxPathInfo[]> [<CommonParameters>]
```

### Object
```
Get-Hash [-Algorithm <String>] [-StringEncoding <StringEncodingParameter>] -InputObject <PSObject>
 [<CommonParameters>]
```

### LiteralPath
```
Get-Hash [-Algorithm <String>] [-LiteralPath] <PscxPathInfo[]> [<CommonParameters>]
```

## DESCRIPTION
Gets the hash value for the specified file or byte array via the pipeline. 
The default hash algorithm is MD5, although you can specify other algorithms using the -Algorithm parameter (MD5, SHA1, SHA256, SHA384, SHA512 and RIPEMD160). 
This cmdlet emits a HashInfo object that has properties for Path, Algorithm, HashString and Hash.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\PS> Get-Hash $PSHOME\PowerShell.exe
        Algorithm: MD5

        Path       : C:\Windows\System32\WindowsPowerShell\v1.0\PowerShell.exe
        HashString : E22825B10BE3E8709BA1AB4D2DF36B57
```

Gets the MD5 hash (default hash algorithm) of the PowerShell executable.

### EXAMPLE 2
PS C:\\\>

```
C:\PS> Get-Hash $PSHOME\PowerShell.exe -Algorithm SHA1
        Algorithm: SHA1

        Path       : C:\Windows\System32\WindowsPowerShell\v1.0\PowerShell.exe
        HashString : 3BA6DDF13A5DEDE95D427E7EFFEDFBC6F1BB267D
```

Gets the SHA1 hash of the PowerShell executable.

### EXAMPLE 2
PS C:\\\>

```
C:\PS> "Hello" | Get-Hash -Algorithm SHA1 -StringEncoding Ascii
        Algorithm: SHA1

        Path       :
        HashString : F7FF9E8B7BB2E09B70935A5D785E0CC5D9D0ABF0
```

Gets the SHA1 hash of the string "Hello" interpreted as Ascii characters.

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

### -Algorithm
Specifies the hash algorithm to use. 
Valid values are MD5 (default), SHA1, SHA256, SHA384, SHA512, RIPEMD160

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: MD5
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
Default value: Unicode
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
