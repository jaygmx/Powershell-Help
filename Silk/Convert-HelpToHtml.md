---
external help file: Silk-help.xml
Module Name: Silk
online version: https://daringfireball.net/projects/markdown/
schema: 2.0.0
---

# Convert-HelpToHtml

## SYNOPSIS
Converts a command's help topic to HTML.

## SYNTAX

```
Convert-HelpToHtml [-Name] <String[]> [[-DisplayName] <String>] [[-Syntax] <String[]>] [[-ModuleName] <String>]
 [[-Script] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
The \`Convert-HelpToHtml\` function convert's a command's help topic to HTML.
This HTML can then be used in a complete HTML page.
It will output the following parts of a help topic, in the following order:

 * Name (in an \`h1\` element).
You can override this name with the \`DisplayName\` parameter.
 * Synopsis
 * Syntax (which you can override with the \`Syntax\` parameter)
 * Description
 * Related Commands (i.e.
\`.LINK\`)
 * Parameters
 * Parameters
 * Input Types (i.e.
\`.INPUTS\`)
 * Return Types (i.e.
\`.OUTPUTS\`)
 * Notes
 * Examples

\`Convert-HelpToHtml\` converts all help text to HTML using \[MarkdownSharp\](https://code.google.com/p/markdownsharp/), a C# \[Markdown\](https://daringfireball.net/projects/markdown/) implementation.
Markdown "allows you to write using an easy-to-read, easy-to-write plain text format, \[that is converted\] to structurally valid XHTML (or HTML)".
This makes your help web-friendly.

If you want to convert an entire module's help to HTML, including any scripts and DSC resources, use the \`Convert-ModuleHelpToHtml\` function.
When converting help for a module, pass the module's name with the \`ModuleName\` parameter, and any of the module's commands or about topics found enclosed in backticks (Markdown's span of code indicators) will be converted to an anchor element whose \`href\` attribute is the command's name with a .html extension.
For example, this help text:

\> Silk's \`Convert-HelpToHtml\` function converts help text written with Markdown into HTML.

would get converted to

\> Silk's \<a href="Convert-HelpToHtml.html"\>Convert-HelpToHtml\</a\> function converts help text written with Markdown into HTML.

\`Convert-HelpToHtml\` assumes you'll take its output, wrap it in a full HTML page, and save all of these generated pages into the same directory.
For example,

    $html = Convert-HelpToHtml -Name 'Convert-HelpToHtml' -ModuleName 'Silk'
    @"
    \<!DOCTYPE html\>
    \<html\>
    \<head\>
        \<title\>Convert-HelpToHTml\</title\>
        \<link href="silk.css" type="text/css" rel="stylesheet" /\>
    \</head\>
    \<body\>
    $html
    \</body\>
    \</html\>
    "@ | Set-Content -Path (Join-Path -Path $webRoot -ChildPath 'Convert-HelpToHtml.html')

\`Convert-HelpToHtml\` outputs HTML 5 (or tries to).
For the best cross-browser compatability, make sure you define a doctype on each page.
This is especially important for Internet Explorer.
If you don't use a doctype, IE will display your pages in quirks mode, which won't display things correctly.

Silk ships with a default cascading stylesheet (CSS) in the \`Resources\` directory.
Copy this file into your webroot and link to it in each of your pages (via the \`link\` tag).
To customize the appearance of your pages, we recommend you create your own stylesheet and link to it in each of your pages.
Make all your style changes in yoru stylesheet.
Future versions of Silk will contain fixes/enhancements to the default stylesheet.
Using your own will make upgrading easier.

## EXAMPLES

### EXAMPLE 1
```
Convert-HelpToHtml -Name 'Get-Module'
```

Demonstrates how to use \`Convert-HelpToHtml\` to generate help for a command.
You can pass multiple command names to the \`Name\` parameter.

### EXAMPLE 2
```
Get-Command -Module 'Silk' | Convert-HelpToHtml -ModuleName 'Silk'
```

Demonstrates how you can pipe commands to \`Convert-HelpToHtml\` to generate help for them.

### EXAMPLE 3
```
Convert-HelpToHtml -Name 'Set-TargetResource' -DisplayName 'My_Dsc_Resource' -Syntax (Get-DscResource -Name 'My_Dsc_Resource' -Syntax)
```

Demonstrates how you can document DSC resources.
In this case, the resource's \`Set-TargetResource\` function contains the help to convert.
Because the syntax for using a DSC resource is different than a PowerShell function/cmdlet, we pass the resource's syntax with the \`Syntax\` parameter.

## PARAMETERS

### -Name
The name of the command(s) to document.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DisplayName
The display name.
When supplied, it is used as the command's name instead of \`Name\`.
Useful if the command name being documented is different than its public name, e.g.
DSC resources.

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

### -Syntax
The syntax of the command.
Useful when showing syntax for DSC resources.

You can get the syntax for a DSC resource with the \`Get-DscResource\` cmdlet:

    Get-DscResource -Name 'My_Dsc_Resource' -Syntax

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

### -ModuleName
The name of the module whose help is getting converted.
Supplying this value will cause any of the module's cmdlets/functions surrounded by backticks (e.g.
\`Convert-HelpToHtml\`) in help text to get replaced with an HTML link to that command's help topic.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Script
The names of any scripts in the module.
Supplying these values will cause any script names surround in backticks (e.g.
\`script.ps1\`) in help text to get replaced with an HTML link to that script's help topic.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
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

[https://daringfireball.net/projects/markdown/](https://daringfireball.net/projects/markdown/)

[Convert-ModuleHelpToHtml]()

