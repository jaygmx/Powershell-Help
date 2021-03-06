---
external help file: PSDocs-help.xml
Module Name: PSDocs
online version: https://github.com/Microsoft/PSDocs/blob/main/docs/commands/PSDocs/en-US/Invoke-PSDocument.md
schema: 2.0.0
---

# Invoke-PSDocument

## SYNOPSIS
Create markdown from an input object.

## SYNTAX

### Input (Default)
```
Invoke-PSDocument [-Module <String[]>] [-Name <String[]>] [-Tag <String[]>] [-InstanceName <String[]>]
 [-InputObject <PSObject>] [[-Path] <String[]>] [-Format <InputFormat>] [-OutputPath <String>] [-PassThru]
 [-Option <PSDocumentOption>] [-Encoding <MarkdownEncoding>] [-Culture <String[]>] [-Convention <String[]>]
 [<CommonParameters>]
```

### InputPath
```
Invoke-PSDocument -InputPath <String[]> [-Module <String[]>] [-Name <String[]>] [-Tag <String[]>]
 [-InstanceName <String[]>] [[-Path] <String[]>] [-Format <InputFormat>] [-OutputPath <String>] [-PassThru]
 [-Option <PSDocumentOption>] [-Encoding <MarkdownEncoding>] [-Culture <String[]>] [-Convention <String[]>]
 [<CommonParameters>]
```

## DESCRIPTION
Create markdown from an input object using a document definition.
Document definitions are discovered within files ending in \`.Doc.ps1\`.
By default, definitions will be be discovered from the current working path.
Use \`-Module\` to discover definitions from modules.

A document is defined using the \`Document\` keyword.

## EXAMPLES

### Example 1
```
# Create a new document definition called Sample in Sample.Doc.ps1
Set-Content -Path .\Sample.Doc.ps1 -Value @'
Document Sample {

    # Add an introduction section
    Section Introduction {

        # Add a comment
        "This is a sample file list from $TargetObject"

        # Generate a table
        Get-ChildItem -Path $TargetObject | Table -Property Name,PSIsContainer
    }
}
'@

# Discover document definitions in the current working path (and subdirectories) within .Doc.ps1 files
Invoke-PSDocument -Path .;
```

Create markdown using *.Doc.ps1 files loaded from the current working directory.

### Example 2
```
# Create a new document definition called Sample in Sample.Doc.ps1
Set-Content -Path .\Sample.Doc.ps1 -Value @'
Document Sample {

    $object = $InputObject
    # Add an introduction section
    Section $InputObject.name {

        # Add a comment
        "This is a sample file list from $InputObject.folder"

        # Generate a table
        Get-ChildItem -Path $InputObject.folder | Table -Property Name,PSIsContainer
    }
}
'@
#Create PSObject with info we want to pass into markdown
$PSDocsInputObject = New-Object PSObject -property @{
    'name' = 'foldername'
    'folder' = 'C:\testfolder'
}

# Create document based on Sample.Doc.ps1 passing PSObject
Invoke-PSDocument -Path .\Sample.Doc.ps1 -InputObject $PSDocsInputObject;
```

Create markdown using a Doc.ps1 file, passing a PSObject in to generate dynamic content.

## PARAMETERS

### -Module
Get document definitions in the specified modules.
When specified, only document definitions from modules will be used.
To additionally use document definitions in paths use \`-Path\` together with \`-Module\`.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: m

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The name of a specific document definitions to use.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: n

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tag
One or more tags that the document definition must contain.
If more then one tag is specified, all tags be present on the document definition to be evaluated.

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

### -InstanceName
The name of the resulting markdown file.
During execution of this command, the variable \`$InstanceName\` will be available within the document definition for use by expressions.

If InstanceName is not specified the name of the document definition will be used instead.
If more then one InstanceName is specified, multiple markdown files will be generated in the order they were specified.

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

### -Format
Configures the input format for when a string is passed in as a target object.

When the \`-InputObject\` parameter or pipeline input is used, strings are treated as plain text by default.
Set this option to either \`Yaml\`, \`Json\`, \`PowerShellData\` to have PSDocs deserialize the object.

When the \`-InputPath\` parameter is used with a file path or URL.
If the Detect format is used, the file extension will be used to automatically detect the format.
When \`-InputPath\` is not used, \`Detect\` is the same as \`None\`.

See \`about_PSDocs_Options\` for details.

This parameter takes precedence over the \`Input.Format\` option if set.

```yaml
Type: PSDocs.Configuration.InputFormat
Parameter Sets: (All)
Aliases: InputFormat
Accepted values: None, Yaml, Json, PowerShellData, Detect

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputPath
Instead of processing objects from the pipeline, import objects file the specified file paths.

```yaml
Type: System.String[]
Parameter Sets: InputPath
Aliases: f

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
An input object that will be passed to each document and can be referenced within document blocks as \`$TargetObject\`.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: Input
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OutputPath
The directory path to store markdown files created based on the specified document template.
This path will be automatically created if it doesn't exist.

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

### -PassThru
When specified generated markdown will be returned to the pipeline instead of being written to file.

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

### -Option
Additional options that configure PSDocs.
A \`PSDocumentOption\` can be created by using the \`New-PSDocumentOption\` cmdlet.
Alternatively a hashtable or path to YAML file can be specified with options.

```yaml
Type: PSDocs.Configuration.PSDocumentOption
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Encoding
Specifies the file encoding for generated markdown files.
By default, UTF-8 without byte order mark (BOM) will be used.
To use UTF-8 with BOM specify \`UTF8\`.

```yaml
Type: PSDocs.Configuration.MarkdownEncoding
Parameter Sets: (All)
Aliases:
Accepted values: Default, UTF8, UTF7, Unicode, UTF32, ASCII

Required: False
Position: Named
Default value: Default
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
A list of paths to use document definitions from.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: p

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Culture
A list of cultures for building documents such as en-AU , and en-US .
Documents are written to culture specific subdirectories when multiple cultures are generated.

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

### -Convention
Specifies the name of conventions to execute during document generation.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Management.Automation.PSObject
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS

[New-PSDocumentOption]()

