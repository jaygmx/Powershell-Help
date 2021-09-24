---
external help file: PSScriptTools-help.xml
Module Name:
online version: http://bit.ly/31SLU7X
schema: 2.0.0
---

# Convert-HashtableToCode

## SYNOPSIS
Convert a hashtable to a string representation.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Convert-HashtableToCode [-Hashtable] <Hashtable> [-Indent <Int32>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Convert-HashtableToCode [-Hashtable] <Hashtable> [-Inline] [<CommonParameters>]
```

## DESCRIPTION
Use this command to convert a hashtable into its text or string equivalent.
It is assumed that any array values contain items of the same type.
This command has not been tested with large or complex hashtables, so you might need to manually edit the output to meet your tastes or requirements.

## EXAMPLES

### Example 1
```
PS C:\> $h = @{Name="SRV1";Asset=123454;Location="Omaha"}
PS C:\> Convert-HashtableToCode $h
@{
        Name = 'SRV1'
        Asset = 123454
        Location = 'Omaha'
}
```

Convert a hashtable object to a string equivalent that you can copy into your script.

### Example 2
```
PS C:\> Convert-HashtableToCode $h -inline

@{Name = 'SRV1';Asset = 123454;Location = 'Omaha'}
```

Create an inline string version of the hashtable.

## PARAMETERS

### -Hashtable
A hashtable to convert.
It can be standard or ordered hashtable.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Indent
Specify the number of tabs to indent.
You shouldn't need to specify this parameter.
It exists for situations where there are nested hashtables.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: tab

Required: False
Position: Named
Default value: 1
Accept pipeline input: False
Accept wildcard characters: False
```

### -Inline
Write the hashtable as an inline expression.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

### System.Collections.Hashtable
## OUTPUTS

### System.String
## NOTES
* Learn more about PowerShell: http://jdhitsolutions.com/blog/essential-powershell-resources/

## RELATED LINKS

[Convert-HashtableString]()

