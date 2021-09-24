---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-PSSnapinHelp

## SYNOPSIS
PSCX Cmdlet: Generates a XML file containing all documentation data.

## SYNTAX

### Path (Default)
```
Get-PSSnapinHelp -LocalizedHelpPath <PscxPathInfo> -OutputPath <PscxPathInfo> [-Path] <PscxPathInfo[]>
 [<CommonParameters>]
```

### Object
```
Get-PSSnapinHelp -LocalizedHelpPath <PscxPathInfo> -OutputPath <PscxPathInfo> -InputObject <PSObject>
 [<CommonParameters>]
```

### LiteralPath
```
Get-PSSnapinHelp -LocalizedHelpPath <PscxPathInfo> -OutputPath <PscxPathInfo> [-LiteralPath] <PscxPathInfo[]>
 [<CommonParameters>]
```

## DESCRIPTION
Generates a XML file containing all documentation data.

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

### -LocalizedHelpPath
@{Text=}

```yaml
Type: Pscx.IO.PscxPathInfo
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputPath
@{Text=}

```yaml
Type: Pscx.IO.PscxPathInfo
Parameter Sets: (All)
Aliases:

Required: True
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
