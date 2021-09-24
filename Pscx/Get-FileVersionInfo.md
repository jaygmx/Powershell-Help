---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-FileVersionInfo

## SYNOPSIS
PSCX Cmdlet: Gets a FileVersionInfo object for the specified path.

## SYNTAX

### Path (Default)
```
Get-FileVersionInfo [-Path] <PscxPathInfo[]> [<CommonParameters>]
```

### LiteralPath
```
Get-FileVersionInfo [-LiteralPath] <PscxPathInfo[]> [<CommonParameters>]
```

## DESCRIPTION
Attempts to get the FileVersionInfo object for the specified path.
Usually only executable files include file version information.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
Get-FileVersionInfo $PSHOME\PowerShell.exe | Format-List *
```

Gets the file version information for PowerShell.exe.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
