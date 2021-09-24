---
external help file: Silk-help.xml
Module Name: Silk
online version: https://bitbucket.org/Swyter/bitbucket-curl-upload-to-repo-downloads
schema: 2.0.0
---

# Split-MarkdownTopic

## SYNOPSIS
Parses a Markdown-formatted module help topic, e.g.
about_Module.

## SYNTAX

```
Split-MarkdownTopic [-ConfigFileRoot] <Object> [-TopicInfo] <Object> [<CommonParameters>]
```

## DESCRIPTION
A Markdown-formatted help topic should contain four sections, \`Topic\`, \`Short Description\`, \`Long Description\`, and \`See Also\`. 
These should all be formatted as level-1 headings. 
For example:

    # Topic

    about_Silk

    # Short Description

    Silk is a PowerShell module used to convert another module's help system into an HTML website.

    # Long Description

    MOre details here. 
Yadda, yadda, yadda.

    # See Also

    about_Silk_AdditionalTopic

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -ConfigFileRoot
The root where the config file was found.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TopicInfo
An object containing information about the topic to parse.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
