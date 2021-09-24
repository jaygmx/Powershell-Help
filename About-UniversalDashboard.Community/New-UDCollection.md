---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDCollection.md
schema: 2.0.0
---

# New-UDCollection

## SYNOPSIS
Creates a collection of items.

## SYNTAX

```
New-UDCollection [[-Id] <String>] [[-Content] <ScriptBlock>] [[-Header] <String>] [-LinkCollection]
 [<CommonParameters>]
```

## DESCRIPTION
Creates a collection of items.

## EXAMPLES

### Collection
```
New-UDCollection -Content {
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

### -Content
Content for the collection.
This should be generated using calls to New-UDCollectionItem.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Header
Header text for collection.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The ID for this collection.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LinkCollection
Whether or not this collection contains links.

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

### None
## OUTPUTS

### System.Object
## NOTES
*

## RELATED LINKS
