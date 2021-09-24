---
external help file: Silk-help.xml
Module Name: Silk
online version: https://daringfireball.net/projects/markdown/
schema: 2.0.0
---

# New-ModuleHelpIndex

## SYNOPSIS
Creates an index page for a module's help.

## SYNTAX

```
New-ModuleHelpIndex [-ModuleName] <String> [[-Script] <String[]>] [[-TagsJsonPath] <String>]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```



## PARAMETERS

### -ModuleName
The name of the module whose index page to create.

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
The names of any scripts that should be included.

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

### -TagsJsonPath
The path to the tags file.
If not provided, no tag tab is generated.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
