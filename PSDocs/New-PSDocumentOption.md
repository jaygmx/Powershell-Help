---
external help file: PSDocs-help.xml
Module Name: PSDocs
online version: https://github.com/Microsoft/PSDocs/blob/main/docs/commands/PSDocs/en-US/New-PSDocumentOption.md
schema: 2.0.0
---

# New-PSDocumentOption

## SYNOPSIS
Create options to configure document generation.

## SYNTAX

### FromPath (Default)
```
New-PSDocumentOption [-Path <String>] [-Format <InputFormat>] [-InputObjectPath <String>]
 [-InputPathIgnore <String[]>] [-Encoding <MarkdownEncoding>] [-Culture <String[]>] [-OutputPath <String>]
 [<CommonParameters>]
```

### FromOption
```
New-PSDocumentOption -Option <PSDocumentOption> [-Format <InputFormat>] [-InputObjectPath <String>]
 [-InputPathIgnore <String[]>] [-Encoding <MarkdownEncoding>] [-Culture <String[]>] [-OutputPath <String>]
 [<CommonParameters>]
```

### FromDefault
```
New-PSDocumentOption [-Default] [-Format <InputFormat>] [-InputObjectPath <String>]
 [-InputPathIgnore <String[]>] [-Encoding <MarkdownEncoding>] [-Culture <String[]>] [-OutputPath <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The New-PSDocumentOption cmdlet creates an options object that can be passed to PSDocs cmdlets to configure document generation behaviour.

## EXAMPLES

### Example 1
```
PS C:\> $option = New-PSDocumentOption -Option @{ 'Markdown.WrapSeparator' = '<br />' };
PS C:\> Invoke-PSDocument -Name 'Sample' -Option $option;
```

Create markdown using the Sample documentation definition using a wrap separator of \`\<br /\>\`.

## PARAMETERS

### -Option
Additional options that configure document generation.
Option also accepts a hashtable to configure options.

```yaml
Type: PSDocs.Configuration.PSDocumentOption
Parameter Sets: FromOption
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
The path to a YAML file containing options.

```yaml
Type: System.String
Parameter Sets: FromPath
Aliases:

Required: False
Position: Named
Default value: .\ps-docs.yaml
Accept pipeline input: False
Accept wildcard characters: False
```

### -Default
When specified, defaults are used for any options not overridden.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FromDefault
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Format
Sets the \`Input.Format\` option to configure the input format for when a string is passed in as a target object.
See about_PSDocs_Options for more information.

```yaml
Type: PSDocs.Configuration.InputFormat
Parameter Sets: (All)
Aliases: InputFormat
Accepted values: None, Yaml, Json, PowerShellData, Detect

Required: False
Position: Named
Default value: Detect
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObjectPath
Sets the \`Input.ObjectPath\` option to use an object path to use instead of the pipeline object.
See about_PSDocs_Options for more information.

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

### -InputPathIgnore
Sets the \`Input.PathIgnore\` option.
If specified, files that match the path spec will not be processed.
See about_PSDocs_Options for more information.

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

### -Encoding
Sets the option \`Markdown.Encoding\`.
Specifies the file encoding for generated markdown files.
By default, UTF-8 without byte order mark (BOM) will be used.
See about_PSDocs_Options for more information.

```yaml
Type: PSDocs.Configuration.MarkdownEncoding
Parameter Sets: (All)
Aliases: MarkdownEncoding
Accepted values: Default, UTF8, UTF7, Unicode, UTF32, ASCII

Required: False
Position: Named
Default value: Default
Accept pipeline input: False
Accept wildcard characters: False
```

### -Culture
Sets the option \`Output.Culture\`.
Specifies a list of cultures for building documents such as en-AU , and en-US .
See about_PSDocs_Options for more information.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: OutputCulture

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputPath
Sets the option \`Output.Path\`.
The option specified one or more custom field bindings.
See about_PSDocs_Options for more information.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### PSDocs.Configuration.PSDocumentOption
## NOTES

## RELATED LINKS

[Invoke-PSDocument]()

