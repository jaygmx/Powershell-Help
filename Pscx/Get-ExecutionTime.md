---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-ExecutionTime

## SYNOPSIS
Gets the execution time for the specified Id of a command in the current
session history.

## SYNTAX

```
Get-ExecutionTime [[-Id] <Int64>] [<CommonParameters>]
```

## DESCRIPTION
Gets the execution time for the specified Id of a command in the current
session history.

## EXAMPLES

### EXAMPLE 1
```
Get-ExecutionTime 1
```

Gets the execution time for id #1 in the session history.

### EXAMPLE 2
```
Get-ExecutionTime
```

Gets the execution time for all commands in the session history.

## PARAMETERS

### -Id
Specifies the Id of the command to retrieve the execution time. 
If no
Id is specified, then the execution time for all commands in the history
is displayed.

```yaml
Type: System.Int64
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
