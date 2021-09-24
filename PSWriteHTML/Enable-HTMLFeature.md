---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# Enable-HTMLFeature

## SYNOPSIS
Provides a way to enable existing feature or extending PSWriteHTML

## SYNTAX

```
Enable-HTMLFeature [[-Feature] <String[]>] [[-Configuration] <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION
Provides a way to enable existing feature or extending PSWriteHTML

## EXAMPLES

### EXAMPLE 1
```
Enable-HTMLFeature -Feature Raphael, Mapael, Jquery, JQueryMouseWheel, "MapaelMaps_$Map" -Configuration $Script:Configuration
```

## PARAMETERS

### -Feature
Choose one of the existing features or define them via extension

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Configuration
Provide hashtable with configuration of libraries

```yaml
Type: System.Collections.IDictionary
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
General notes

## RELATED LINKS
