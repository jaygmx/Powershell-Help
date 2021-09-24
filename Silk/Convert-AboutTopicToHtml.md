---
external help file: Silk-help.xml
Module Name: Silk
online version:
schema: 2.0.0
---

# Convert-AboutTopicToHtml

## SYNOPSIS
Converts an about topic into HTML.

## SYNTAX

```
Convert-AboutTopicToHtml [-InputObject] <Object> [[-TopicName] <String>] [-ModuleName] <String>
 [[-TopicHeading] <String>] [[-ShortDescriptionHeading] <String>] [[-LongDescriptionHeading] <String>]
 [[-SeeAlsoHeading] <String>] [[-HeadingMap] <Hashtable>] [[-Script] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
The \`Convert-AboutTopicToHtml\` converts a PowerShell about topic into HTML.
The about topic is expected to be \[formatted like PowerShell's internal topics\](https://msdn.microsoft.com/en-us/library/Dd878343.aspx):

    TOPIC
        about_\<subject or module name\>
    
    SHORT DESCRIPTION
        A short, one-line description of the topic contents.
    
    LONG DESCRIPTION
        A detailed, full description of the subject or purpose of the module.
    
    EXAMPLES
        Examples of how to use the module or how the subject feature works in practice.
    
    KEYWORDS
        Terms or titles on which you might expect your users to search for the information in this topic.
    
    SEE ALSO
        Text-only references for further reading.
Hyperlinks cannot work in the Windows PowerShell console. 

\`Convert-AboutTopicToHtml\` does the following:

 * Removes the \`TOPIC\` AND \`SHORT DESCRIPTION\` headers
 * Wraps the topic name in an \<h1\> tag
 * Renames the \`LONG DESCRIPTION\` heading to '\<h2\>Description\</h2\>
 * Wraps all other headers in \<h2\> elements.
 * Converts the bodies of each section to HTML 

Lines that don't begin with spaces are assumed to be headers.

Lines that begin with spaces are assumed to be content written in Markdown.

The \`SEE ALSO\` section is parsed, one line at a time for links, command names, and other help topics, e.g.

    SEE ALSO
        https://msdn.microsoft.com/en-us/library/Dd878343.aspx
        about_Silk
        Convert-AboutTopicToHtml

Would convert into a three item list, the first a link to the web, the second a link to the \`about_Silk.html\` topic, and the third to the \`Convert-AboutTopicToHtml.html\` page.

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -InputObject
The name of the help topic, include the \`about_\` prefix, or a \`FileInfo\` object representing the help topic, or the help topic as a giant string.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TopicName
The name of the topic you're converting.
Only used if \`InputObject\` is the text of the about topic.

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

### -ModuleName
The name of the module being documented.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TopicHeading
The heading used for the topic's name.
Default is \`TOPIC\`.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: TOPIC
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShortDescriptionHeading
The heading used for the topic's short description.
Default is \`SHORT DESCRIPTION\`.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: SHORT DESCRIPTION
Accept pipeline input: False
Accept wildcard characters: False
```

### -LongDescriptionHeading
The heading used for the topic's long description.
Default is \`LONG DESCRIPTION\`.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: LONG DESCRIPTION
Accept pipeline input: False
Accept wildcard characters: False
```

### -SeeAlsoHeading
The heading used for the topic's \`See Also\` section.
Default is \`SEE ALSO\`.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: SEE ALSO
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeadingMap
A hashtable of headings to use.
They key should be the section name.
The value should be the heading name.

```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
Default value: @{}
Accept pipeline input: False
Accept wildcard characters: False
```

### -Script
The names of any scripts in the module.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
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
