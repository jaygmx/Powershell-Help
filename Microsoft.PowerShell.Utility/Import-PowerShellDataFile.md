---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
Module Name: Microsoft.PowerShell.Utility
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/import-powershelldatafile?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Import-PowerShellDataFile

## SYNOPSIS
Imports values from a \`.PSD1\` file without invoking its contents.

## SYNTAX

### ByPath (Default)
```
Import-PowerShellDataFile [-Path] <String[]> [-SkipLimitCheck] [<CommonParameters>]
```

### ByLiteralPath
```
Import-PowerShellDataFile [-LiteralPath] <String[]> [-SkipLimitCheck] [<CommonParameters>]
```

## DESCRIPTION
The \`Import-PowerShellDataFile\` cmdlet safely imports key-value pairs from hashtables defined in a \`.PSD1\` file.
The values could be imported using \`Invoke-Expression\` on the contents of the file.
However, \`Invoke-Expression\` runs any code contained in the file.
This could produce unwanted results or execute unsafe code.
\`Import-PowerShellDataFile\` imports the data without invoking the code.

## EXAMPLES

### Example 1: Retrieve values from PSD1
```
Get-Content .\Configuration.psd1
$config = Import-PowerShellDataFile .\Configuration.psd1
$config.AllNodes

@{
    AllNodes = @(
        @{
            NodeName = 'DSC-01'
        }
        @{
            NodeName = 'DSC-02'
        }
    )
}

Name                           Value
----                           -----
NodeName                       DSC-01
NodeName                       DSC-02
```

## PARAMETERS

### -LiteralPath
The path to the file being imported.
All characters in the path are treated as literal values.
Wildcard characters are not processed.

```yaml
Type: System.String[]
Parameter Sets: ByLiteralPath
Aliases: PSPath, LP

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
The path to the file being imported.
Wildcards are allowed but only the first matching file is imported.

```yaml
Type: System.String[]
Parameter Sets: ByPath
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkipLimitCheck


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### System.Collections.Hashtable
## NOTES

## RELATED LINKS

[Invoke-Expression]()

[Import-LocalizedData]()

