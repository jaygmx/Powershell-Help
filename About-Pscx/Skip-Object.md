---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Skip-Object

## SYNOPSIS
PSCX Cmdlet: Skips the specified objects in the pipeline.

## SYNTAX

```
Skip-Object [[-First] <Int32>] [[-Last] <Int32>] [-InputObject <PSObject>] [[-Index] <Int32[]>]
 [<CommonParameters>]
```

## DESCRIPTION
Skips the specified number of objects at the beginning of a sequence and/or the end of a sequence.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
0..20 | Skip-Object -first 5 -last 2 -index 10,11
```

This command will prevent the first five objects, the last two objects and the objects at index 10 and 11 from being output by the pipeline.

## PARAMETERS

### -First
Skips the selected number of objects at the head of the pipeline sequence.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Last
Skips the selected number of objects at the tail of the pipeline sequence.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Accepts an object as input to the cmdlet.
Enter a variable that contains the objects or type a command or expression that gets the objects.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Index
Skips objects at the selected indices within the pipeline sequence.

```yaml
Type: Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Object[]
## OUTPUTS

### PSobject
## NOTES
*

## RELATED LINKS
