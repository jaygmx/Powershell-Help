---
external help file: Google.PowerShell.dll-Help.xml
Module Name: GoogleCloud
online version:
schema: 2.0.0
---

# Publish-GcpsMessage

## SYNOPSIS


## SYNTAX

### DataAndAttributes (Default)
```
Publish-GcpsMessage [-Project <String>] [-Topic] <String> [-Data <String>] [-Attributes <Hashtable>]
 [<CommonParameters>]
```

### Message
```
Publish-GcpsMessage [-Project <String>] [-Topic] <String> -Message <PubsubMessage[]> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Attributes


```yaml
Type: System.Collections.Hashtable
Parameter Sets: DataAndAttributes
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Data


```yaml
Type: System.String
Parameter Sets: DataAndAttributes
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Message


```yaml
Type: Google.Apis.Pubsub.v1.Data.PubsubMessage[]
Parameter Sets: Message
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Project


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

### -Topic


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
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

## RELATED LINKS
