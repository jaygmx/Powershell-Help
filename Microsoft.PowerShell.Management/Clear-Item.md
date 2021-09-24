---
external help file: Microsoft.PowerShell.Commands.Management.dll-Help.xml
Module Name: Microsoft.PowerShell.Management
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.management/clear-item?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Clear-Item

## SYNOPSIS
Clears the contents of an item, but does not delete the item.

## SYNTAX

### Path (Default)
```
Clear-Item [-Path] <String[]> [-Force] [-Filter <String>] [-Include <String[]>] [-Exclude <String[]>]
 [-Credential <PSCredential>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### LiteralPath
```
Clear-Item -LiteralPath <String[]> [-Force] [-Filter <String>] [-Include <String[]>] [-Exclude <String[]>]
 [-Credential <PSCredential>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The \`Clear-Item\` cmdlet clears the content of an item, but it does not delete the item.
For example, the \`Clear-Item\` cmdlet can delete the value of a variable, but it does not delete the variable.
The value that used to represent a cleared item is defined by each PowerShell provider.
This cmdlet is similar to \`Clear-Content\`, but it works on aliases and variables, instead of files.

## EXAMPLES

### Example 1: Clear the value of a variable
```
Clear-Item Variable:TestVar1

Set-Location Variable:
PS Variable:\> Clear-Item TestVar1
```

### Example 2: Clear all registry entries
```
Clear-Item HKLM:\Software\MyCompany\MyKey -Confirm
```

## PARAMETERS

### -Credential
\> \[!NOTE\] \> This parameter is not supported by any providers installed with PowerShell.
\> To impersonate another user, or elevate your credentials when running this cmdlet, \> use Invoke-Command (../Microsoft.PowerShell.Core/Invoke-Command.md).

```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Current user
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Exclude
Specifies, as a string array, an item or items that this cmdlet excludes in the operation.
The value of this parameter qualifies the Path parameter.
Enter a path element or pattern, such as \` .txt\`.
Wildcard characters are permitted.
The Exclude * parameter is effective only when the command includes the contents of an item, such as \`C:\Windows*\`, where the wildcard character specifies the contents of the \`C:\Windows\` directory.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filter
Specifies a filter to qualify the Path parameter.
The FileSystem (../Microsoft.PowerShell.Core/About/about_FileSystem_Provider.md)provider is the only installed PowerShell provider that supports the use of filters.
You can find the syntax for the FileSystem filter language in about_Wildcards (../Microsoft.PowerShell.Core/About/about_Wildcards.md).
Filters are more efficient than other parameters, because the provider applies them when the cmdlet gets the objects rather than having PowerShell filter the objects after they are retrieved.

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

### -Force
Indicates that the cmdlet clears items that cannot otherwise be changed, such as read- only aliases.
The cmdlet cannot clear constants.
Implementation varies from provider to provider.
For more information, see about_Providers (../Microsoft.PowerShell.Core/About/about_Providers.md).
The cmdlet cannot override security restrictions, even when the Force parameter is used.

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

### -Include
Specifies, as a string array, an item or items that this cmdlet includes in the operation.
The value of this parameter qualifies the Path parameter.
Enter a path element or pattern, such as \`" .txt"\`.
Wildcard characters are permitted.
The Include * parameter is effective only when the command includes the contents of an item, such as \`C:\Windows*\`, where the wildcard character specifies the contents of the \`C:\Windows\` directory.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LiteralPath
Specifies a path to one or more locations.
The value of LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell PowerShell not to interpret any characters as escape sequences.

For more information, see about_Quoting_Rules (../Microsoft.Powershell.Core/About/about_Quoting_Rules.md).

```yaml
Type: System.String[]
Parameter Sets: LiteralPath
Aliases: PSPath, LP

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Specifies the path to the items being cleared.
Wildcard characters are permitted.
This parameter is required, but the parameter name Path is optional.

```yaml
Type: System.String[]
Parameter Sets: Path
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
You can pipe a path string to this cmdlet.

## OUTPUTS

### None
This cmdlet does not generate any output.

## NOTES
- The \`Clear-Item\` cmdlet is supported only by several PowerShell providers, including the Alias , Environment , Function , Registry , and Variable providers. As such, you can use   \`Clear-Item\` to delete the content of items in the provider namespaces. To list the providers   available in your session, type \`Get-PsProvider\`. For more information, see about_Providers (../Microsoft.PowerShell.Core/About/about_Providers.md). - You cannot use \`Clear-Item\` to delete the contents of a file, because the PowerShell FileSystem   provider does not support this cmdlet. To clear files, use the \`Clear-Content\`.

## RELATED LINKS

[Copy-Item]()

[Get-Item]()

[Invoke-Item]()

[Move-Item]()

[New-Item]()

[Remove-Item]()

[Rename-Item]()

[Set-Item]()

[about_Providers]()

