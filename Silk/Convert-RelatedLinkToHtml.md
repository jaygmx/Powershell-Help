---
external help file: Silk-help.xml
Module Name: Silk
online version: https://daringfireball.net/projects/markdown/
schema: 2.0.0
---

# Convert-RelatedLinkToHtml

## SYNOPSIS
Converts a command's related link to HTML.

## SYNTAX

```
Convert-RelatedLinkToHtml [-CommandHelp] <Object> [[-ModuleName] <String>] [[-Script] <String[]>]
 [<CommonParameters>]
```

## DESCRIPTION
\`Convert-RelatedLinkToHtml\` converts a command's related links to HTML.
If the related link is not a URL, the command name is converted to a link that poitns to a \`CommandName.html\` file.

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -CommandHelp
The help object returned by \`Get-Help\`.

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
The name of the module the command is in.

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

### -Script
The names of any scripts in the module.

```yaml
Type: System.String[]
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

## OUTPUTS

## NOTES

## RELATED LINKS
