---
external help file: Silk-help.xml
Module Name: Silk
online version: https://daringfireball.net/projects/markdown/
schema: 2.0.0
---

# Edit-HelpText

## SYNOPSIS
Converts the command names in a block of text to links.

## SYNTAX

```
Edit-HelpText [-InputObject] <Object> [[-ModuleName] <String>] [<CommonParameters>]
```

## DESCRIPTION
The \`Edit-HelpText\` function converts all a module's command names or help topic names into Markdown links.
The command names or help topic names should be surrounded by backticks, e.g.
\`Invoke-Function\`, \`about_Module\`.

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```



## PARAMETERS

### -InputObject
The text to convert.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ModuleName
The name of the module whose command names to convert.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
