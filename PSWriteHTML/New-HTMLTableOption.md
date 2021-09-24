---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLTableOption

## SYNOPSIS
Configures New-HTMLTable options

## SYNTAX

```
New-HTMLTableOption [[-DataStore] <String>] [-BoolAsString] [-NumberAsString] [[-DateTimeFormat] <String>]
 [[-NewLineCarriage] <String>] [[-NewLine] <String>] [[-Carriage] <String>] [-ArrayJoin]
 [[-ArrayJoinString] <String>] [<CommonParameters>]
```

## DESCRIPTION
Configures New-HTMLTable options

## EXAMPLES

### EXAMPLE 1
```
New-HTML {
    New-HTMLTableOption -DateTimeFormat "yyyy-MM-dd HH:mm:ss" -BoolAsString
    New-HTMLSection -Invisible {
        New-HTMLSection -HeaderText 'Standard Table with PSCustomObjects' {
            New-HTMLTable -DataTable $DataTable1
        }
        New-HTMLSection -HeaderText 'Standard Table with PSCustomObjects' {
            New-HTMLTable -DataTable $DataTable1 -DataStore JavaScript
        }
    }
} -ShowHTML
```

## PARAMETERS

### -DataStore
Choose how Data is stored for all tables HTML, JavaScript or AjaxJSON (external file)

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BoolAsString
When JavaScript or AjaxJSON is used, forces bool to string

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

### -NumberAsString
When JavaScript or AjaxJSON is used, forces number to string

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

### -DateTimeFormat
When JavaScript or AjaxJSON is used, one can configure DateTimeFormat (in PowerShell way)

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NewLineCarriage
When JavaScript or AjaxJSON is used, one can configure NewLineCarriage.
Default NewLineCarriage = '\<br\>'

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NewLine
When JavaScript or AjaxJSON is used, one can configure NewLine.
Default value for NewLine = "\n"

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Carriage
When JavaScript or AjaxJSON is used, one can configure Carriage.
Default value for Carriage = "\r"

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ArrayJoin
When JavaScript or AjaxJSON is used, forces any array to be a string regardless of depth level

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

### -ArrayJoinString
Uses defined string or char for array join.
By default it uses comma with a space when used.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: ,
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
