---
external help file: Microsoft.PowerShell.Commands.Management.dll-Help.xml
Module Name: Microsoft.PowerShell.Management
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.management/rename-item?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Rename-Item

## SYNOPSIS
Renames an item in a PowerShell provider namespace.

## SYNTAX

### ByPath (Default)
```
Rename-Item [-Path] <String> [-NewName] <String> [-Force] [-PassThru] [-Credential <PSCredential>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### ByLiteralPath
```
Rename-Item -LiteralPath <String> [-NewName] <String> [-Force] [-PassThru] [-Credential <PSCredential>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The \`Rename-Item\` cmdlet changes the name of a specified item.
This cmdlet does not affect the content of the item being renamed.

You can't use \`Rename-Item\` to move an item, such as by specifying a path together with the new name.
To move and rename an item, use the \`Move-Item\` cmdlet.

## EXAMPLES

### Example 1: Rename a file
```
Rename-Item -Path "c:\logfiles\daily_file.txt" -NewName "monday_file.txt"
```

### Example 2: Rename and move an item
```
Rename-Item -Path "project.txt" -NewName "d:\archive\old-project.txt"

Rename-Item : can't rename because the target specified represents a path or device name.
At line:1 char:12
+ Rename-Item <<<<  -path project.txt -NewName d:\archive\old-project.txt
+ CategoryInfo          : InvalidArgument: (:) [Rename-Item], PS>  Move-Item -Path "project.txt" -De
stination "d:\archive\old-project.txt"
```

### Example 3: Rename a registry key
```
Rename-Item -Path "HKLM:\Software\MyCompany\Advertising" -NewName "Marketing"
```

### Example 4: Rename multiple files
```
Get-ChildItem *.txt

Directory: C:\temp\files

Mode                LastWriteTime         Length Name
----                -------------         ------ ----
-a----        10/3/2019   7:47 AM           2918 Friday.TXT
-a----        10/3/2019   7:46 AM           2918 Monday.Txt
-a----        10/3/2019   7:47 AM           2918 Wednesday.txt

Get-ChildItem *.txt | Rename-Item -NewName { $_.Name -replace '.txt','.log' }
Get-ChildItem *.log

Directory: C:\temp\files

Mode                LastWriteTime         Length Name
----                -------------         ------ ----
-a----        10/3/2019   7:47 AM           2918 Friday.log
-a----        10/3/2019   7:46 AM           2918 Monday.log
-a----        10/3/2019   7:47 AM           2918 Wednesday.log
```

The \`Get-ChildItem\` cmdlet gets all the files in the current folder that have a \`.txt\` file extension then pipes them to \`Rename-Item\`.
The value of NewName is a script block that runs before the value is submitted to the NewName parameter.

In the script block, the \`$_\` automatic variable represents each file object as it comes to the command through the pipeline.
The script block uses the \`-replace\` operator to replace the file extension of each file with \`.log\`.
Notice that matching using the \`-replace\` operator is not case sensitive.

## PARAMETERS

### -Credential
\> \[!NOTE\] \> This parameter is not supported by any providers installed with PowerShell.
To impersonate another \> user, or elevate your credentials when running this cmdlet, use Invoke-Command (../Microsoft.PowerShell.Core/Invoke-Command.md).

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

### -Force
Forces the cmdlet to rename items that can't otherwise be changed, such as hidden or read-only files or read-only aliases or variables.
The cmdlet can't change constant aliases or variables.
Implementation varies from provider to provider.
For more information, see about_Providers (../Microsoft.PowerShell.Core/About/about_Providers.md).

Even using the Force parameter, the cmdlet can't override security restrictions.

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

### -LiteralPath
Specifies a path to one or more locations.
The value of LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell PowerShell not to interpret any characters as escape sequences.

For more information, see about_Quoting_Rules (../Microsoft.Powershell.Core/About/about_Quoting_Rules.md).

```yaml
Type: System.String
Parameter Sets: ByLiteralPath
Aliases: PSPath, LP

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -NewName
Specifies the new name of the item.
Enter only a name, not a path and name.
If you enter a path that differs from the path that is specified in the Path parameter, \`Rename-Item\` generates an error.
To rename and move an item, use \`Move-Item\`.

You can't use wildcard characters in the value of the NewName parameter.
To specify a name for multiple files, use the Replace operator in a regular expression.
For more information about the Replace operator, see about_Comparison_Operators (../Microsoft.PowerShell.Core/About/about_Comparison_Operators.md).

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Returns an object that represents the item to the pipeline.
By default, this cmdlet does not generate any output.

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

### -Path
Specifies the path of the item to rename.

```yaml
Type: System.String
Parameter Sets: ByPath
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
You can pipe a string that contains a path to this cmdlet.

## OUTPUTS

### None or an object that represents the renamed item.
This cmdlet generates an object that represents the renamed item, if you specify the PassThru parameter.
Otherwise, this cmdlet does not generate any output.

## NOTES
\`Rename-Item\` is designed to work with the data exposed by any provider.
To list the providers available in your session, type \`Get-PsProvider\`.
For more information, see about_Providers (../Microsoft.PowerShell.Core/About/about_Providers.md).

## RELATED LINKS

[Clear-Item]()

[Copy-Item]()

[Get-ChildItem]()

[Get-Item]()

[Invoke-Item]()

[Move-Item]()

[New-Item]()

[Remove-Item]()

[Rename-ItemProperty]()

[Set-Item]()

[about_Providers]()

