---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-TableColumnOption

## SYNOPSIS
Allows for certain modification of options within DataTable's columnDefs parameter.
You can set visibility, searchability, sortability, and width for specific columns

## SYNTAX

### ColumnIndex (Default)
```
New-TableColumnOption -ColumnIndex <Int32[]> [-Width <String>] [-Hidden <Boolean>] [-Searchable <Boolean>]
 [-Sortable <Boolean>] [<CommonParameters>]
```

### AllColumns
```
New-TableColumnOption [-AllColumns] [-Width <String>] [-Hidden <Boolean>] [-Searchable <Boolean>]
 [-Sortable <Boolean>] [<CommonParameters>]
```

## DESCRIPTION
Allows for certain modification of options within DataTable's columnDefs parameter.
See: https://datatables.net/reference/option/columnDefs

New-HTMLTable has parameters for -ResponsivePriorityOrder and -ResponsivePriorityOrderIndex and these are set at a higher precedent than options specified here.
See the DataTable reference section for conflict resolution.

The New-TableColumnOption cmdlet will add entries to the columnDefs parameter in the order in which the cmdlets are ordered.
If you use 2 or more New-TableColumnOption, the first cmdlet takes priority over the second cmdlet if they specify the same targets or overriding property values
With this in mind, you should almost always specify -AllColumns last, since that will take priority over any commands issued later

## EXAMPLES

### EXAMPLE 1
```
New-TableColumnOption -ColumnIndex (0..4) -Width 50
The first 5 columns with have a width defined as 50, this may not be exact.
See: https://datatables.net/reference/option/columns.width
```

### EXAMPLE 2
```
New-TableColumnOption -ColumnIndex 0,1,2 -Hidden $false
New-TableColumnOption -ColumnIndex 1 -Sortable $true
New-TableColumnOption -AllColumns -Hidden $true -Searchable $false -Sortable $false
All columns will be hidden, not searchable, and not sortable
However, since there is a option specified higher up, the first 3 columns will be visible
Additionally the 2nd column will be sortable
```

## PARAMETERS

### -ColumnIndex
Identifies specific columns that the properties should apply to

```yaml
Type: System.Int32[]
Parameter Sets: ColumnIndex
Aliases: Targets

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllColumns
Uses the columnDef Target "_ALL" to indicate all columns / remaining columns

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: AllColumns
Aliases: AllTargets, TargetAll

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Width
Width for the column as a string

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Hidden
Defines if a column is hidden.
A hidden column can still be used by Conditional Formatting and can still be searchable

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Searchable
Defines if a column is able to be searched

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sortable
Defines if a column can be sorted

```yaml
Type: System.Boolean
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

### None. You cannot pipe objects to New-TableColumnOption
## OUTPUTS

### PSCustomObject
## NOTES
The New-HTMLTable cmdlet has -ResponsivePriorityOrder and -ResponsivePriorityOrderIndex that also modifes the columnDefs option in DataTable

## RELATED LINKS
