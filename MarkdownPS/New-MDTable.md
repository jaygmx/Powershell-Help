---
external help file: MarkdownPS-help.xml
Module Name: MarkdownPS
online version:
schema: 2.0.0
---

# New-MDTable

## SYNOPSIS
This commandlet output a table in markdown syntax

## SYNTAX

```
New-MDTable [-Object] <PSObject[]> [-Columns <Object>] [-NoNewLine] [-Shrink] [<CommonParameters>]
```

## DESCRIPTION
This commandlet output quote in markdown syntax by adding a two rows for the header and then one line per entry in the array.

## EXAMPLES

### EXAMPLE 1
```
Get-Command New-MDTable |Select-Object Name,CommandType | New-MDTable
```

| Name        | CommandType |
| ----------- | ----------- |
| New-MDTable | Function    |

### EXAMPLE 2
```
Get-Command New-MDTable |Select-Object Name,CommandType | New-MDTable -Shrink
```

| Name | CommandType |
| ---- | ----------- |
| New-MDTable | Function |

### EXAMPLE 3
```
Get-Command New-MDTable | New-MDTable -Columns ([ordered]@{Name=$null;CommandType=$null})
```

| Name        | CommandType |
| ----------- | ----------- |
| New-MDTable | Function    |

### EXAMPLE 4
```
Get-Command New-MDTable | New-MDTable -Columns ([ordered]@{CommandType=$null;Name=$null})
```

| CommandType | Name        |
| ----------- | ----------- |
| Function    | New-MDTable |

### EXAMPLE 5
```
Get-Command New-MDTable | New-MDTable -Columns (@{CommandType=$null;Name=$null})
```

| Name        | CommandType |
| ----------- | ----------- |
| New-MDTable | Function    |

### EXAMPLE 6
```
Get-Command New-MDTable | New-MDTable -Columns ([ordered]@{Name="left";CommandType="center";Version="right"})
| Name        | CommandType | Version     |
| ----------- |:-----------:| -----------:|
| New-MDTable | Function    |             |
```

## PARAMETERS

### -Object
Any object

```yaml
Type: System.Management.Automation.PSObject[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Columns
The columns that compose the table.
Columns must be an ordered hashtable \[ordered\]@{} where the keys are the column names and as optional value (left,center,right).

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoNewLine
Controls if a new line is added at the end of the output

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Shrink
Shrinks each row to just actually fill the data

```yaml
Type: System.Management.Automation.SwitchParameter
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

### Any table
## OUTPUTS

### A table representation in markdown
## NOTES
Use the -NoNewLine parameter when you don't want the next markdown content to be separated.

## RELATED LINKS
