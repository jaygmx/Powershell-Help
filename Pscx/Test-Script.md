---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Test-Script

## SYNOPSIS
PSCX Cmdlet: Determines whether a PowerShell script has any syntax errors.

## SYNTAX

### Path (Default)
```
Test-Script [-Context <Int32[]>] [-Path] <PscxPathInfo[]> [<CommonParameters>]
```

### Object
```
Test-Script [-Context <Int32[]>] -InputObject <PSObject> [<CommonParameters>]
```

### LiteralPath
```
Test-Script [-Context <Int32[]>] [-LiteralPath] <PscxPathInfo[]> [<CommonParameters>]
```

## DESCRIPTION
Determines whether a PowerShell script has any syntax errors using the PowerShell script tokenizer.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\PS> Test-Script foo.ps1
```

Displays syntax errors and returns a boolean indicating if there were.

### EXAMPLE 2
PS C:\\\>

```
C:\PS> Test-Script foo.ps1 -WarningAction SilentlyContinue
```

Returns a boolean indicating if there were any syntax errors, suppressing all warnings.

### EXAMPLE 3
PS C:\\\>

```
C:\PS> Test-Script foo.ps1 -Context 1
```

Displays syntax errors as well as the line of script before and after the line containing each syntax error. 
Returns a boolean indicating if there was a syntax error.

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

### -Context
The number of lines of source script to show before and after the line containing the syntax error.

```yaml
Type: System.Int32[]
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

### System.String
## OUTPUTS

### System.Boolean
## NOTES

## RELATED LINKS
