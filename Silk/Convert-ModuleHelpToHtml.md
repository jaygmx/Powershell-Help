---
external help file: Silk-help.xml
Module Name: Silk
online version: https://daringfireball.net/projects/markdown/
schema: 2.0.0
---

# Convert-ModuleHelpToHtml

## SYNOPSIS
Converts a module's help into HTML.

## SYNTAX

```
Convert-ModuleHelpToHtml [-ModuleName] <String> [[-Script] <String[]>] [[-HeadingMap] <Hashtable>]
 [-SkipCommandHelp] [<CommonParameters>]
```

## DESCRIPTION
The \`Convert-ModuleHelpToHtml\` function converts a module's help into HTML.
It returns an object for each command and about help topic in the module.
The object

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -ModuleName
The name of the module whose help to convert.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Script
Any scripts included in the module whose help should get generated.
Scripts are assumed to be in the root of the module.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeadingMap
A hashtable of headings to use.
They key should be the section name.
The value should be the heading name.
Only used when converting about help topics to HTML.

```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkipCommandHelp
Don't generate help for individual commands.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
