---
external help file: Microsoft.PowerShell.Commands.Management.dll-Help.xml
Module Name: Microsoft.PowerShell.Management
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.management/new-itemproperty?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# New-ItemProperty

## SYNOPSIS
Creates a new property for an item and sets its value.

## SYNTAX

### Path (Default)
```
New-ItemProperty [-Path] <String[]> [-Name] <String> [-PropertyType <String>] [-Value <Object>] [-Force]
 [-Filter <String>] [-Include <String[]>] [-Exclude <String[]>] [-Credential <PSCredential>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### LiteralPath
```
New-ItemProperty -LiteralPath <String[]> [-Name] <String> [-PropertyType <String>] [-Value <Object>] [-Force]
 [-Filter <String>] [-Include <String[]>] [-Exclude <String[]>] [-Credential <PSCredential>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The \`New-ItemProperty\` cmdlet creates a new property for a specified item and sets its value.
Typically, this cmdlet is used to create new registry values, because registry values are properties of a registry key item.

This cmdlet does not add properties to an object.

- To add a property to an instance of an object, use the \`Add-Member\` cmdlet.
- To add a property to all objects of a particular type, modify the Types.ps1xml file.

## EXAMPLES

### Example 1: Add a registry entry
```
New-ItemProperty -Path "HKLM:\Software\MyCompany" -Name "NoOfEmployees" -Value 822
Get-ItemProperty "HKLM:\Software\MyCompany"

PSPath        : Microsoft.PowerShell.Core\Registry::HKEY_LOCAL_MACHINE\software\mycompany
PSParentPath  : Microsoft.PowerShell.Core\Registry::HKEY_LOCAL_MACHINE\software
PSChildName   : mycompany
PSDrive       : HKLM
PSProvider    : Microsoft.PowerShell.Core\Registry
NoOfLocations : 2
NoOfEmployees : 822
```

### Example 2: Add a registry entry to a key
```
Get-Item -Path "HKLM:\Software\MyCompany" | New-ItemProperty -Name NoOfLocations -Value 3
```

This command works because the parameter-binding feature of PowerShell associates the path of the \`RegistryKey\` object that \`Get-Item\` returns with the LiteralPath parameter of \`New-ItemProperty\`.
For more information, see about_Pipelines (../Microsoft.PowerShell.Core/About/about_pipelines.md).

### Example 3: Create a MultiString value in the registry using a Here-String
```
$newValue = New-ItemProperty -Path "HKLM:\SOFTWARE\ContosoCompany\" -Name 'HereString' -PropertyType MultiString -Value @"
This is text which contains newlines
It can also contain "quoted" strings
"@
$newValue.multistring

This is text which contains newlines
It can also contain "quoted" strings
```

### Example 4: Create a MultiString value in the registry using an array
```
$newValue = New-ItemProperty -Path "HKLM:\SOFTWARE\ContosoCompany\" -Name 'MultiString' -PropertyType MultiString -Value ('a','b','c')
$newValue.multistring[0]

a
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
Forces the cmdlet to create a property on an object that cannot otherwise be accessed by the user.
Implementation varies from provider to provider.
For more information, see about_Providers (../Microsoft.PowerShell.Core/About/about_Providers.md).

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

### -Name
Specifies a name for the new property.
If the property is a registry entry, this parameter specifies the name of the entry.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: PSProperty

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Specifies the path of the item.
Wildcard characters are permitted.
This parameter identifies the item to which this cmdlet adds the new property.

```yaml
Type: System.String[]
Parameter Sets: Path
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PropertyType
Specifies the type of property that this cmdlet adds.
The acceptable values for this parameter are:

- String : Specifies a null-terminated string. Equivalent to REG_SZ . - ExpandString : Specifies a null-terminated string that contains unexpanded references to   environment variables that are expanded when the value is retrieved. Equivalent to REG_EXPAND_SZ . - Binary : Specifies binary data in any form. Equivalent to REG_BINARY . - DWord : Specifies a 32-bit binary number. Equivalent to REG_DWORD . - MultiString : Specifies an array of null-terminated strings terminated by two null characters.   Equivalent to REG_MULTI_SZ . - Qword : Specifies a 64-bit binary number. Equivalent to REG_QWORD . - Unknown : Indicates an unsupported registry data type, such as REG_RESOURCE_LIST .

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Type

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Value
Specifies the property value.
If the property is a registry entry, this parameter specifies the value of the entry.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### None
You cannot pipe input to this cmdlet.

## OUTPUTS

### System.Management.Automation.PSCustomObject
\`New-ItemProperty\` returns a custom object that contains the new property.

## NOTES
\`New-ItemProperty\` is designed to work with the data exposed by any provider.
To list the providers available in your session, type \`Get-PSProvider\`.
For more information, see about_Providers (../Microsoft.PowerShell.Core/About/about_Providers.md).

## RELATED LINKS

[Clear-ItemProperty]()

[Copy-ItemProperty]()

[Get-ItemProperty]()

[Move-ItemProperty]()

[Remove-ItemProperty]()

[Rename-ItemProperty]()

[Set-ItemProperty]()

[about_Providers]()

