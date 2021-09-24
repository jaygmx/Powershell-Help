---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDCollection.md
schema: 2.0.0
---

# New-UDCollectionItem

## SYNOPSIS
Creates a new collection item.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDCollectionItem [-Active] [-Content <ScriptBlock>] [-Id <String>] [-SecondaryContent <ScriptBlock>]
 [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDCollectionItem [-Active] [-Content <ScriptBlock>] [-Id <String>] [-Url <String>] [<CommonParameters>]
```

## DESCRIPTION
Creates a new collection item.

## EXAMPLES

### Example 1
```
PS C:\> New-UDCollection -Content {
    New-UDCollectionItem -Content { 
        "Item 1"
    }
    New-UDCollectionItem -Content { 
        "Item 2"
    }
    New-UDCollectionItem -Content { 
        "Item 3"
    }
}
```

Creates a collection of 3 items.

## PARAMETERS

### -Active
Whether this collection item is active.

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

### -Content
The content for this collection item.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The ID of this collection item.

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

### -SecondaryContent
Secondary content for this collection item.

```yaml
Type: ScriptBlock
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Url
URL for this collection item.
This should be used when New-UDCollection has the LinksCollection parameter specified.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

### None
## OUTPUTS

### System.Object
## NOTES
*

## RELATED LINKS
