---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Edit-File

## SYNOPSIS
PSCX Cmdlet: Edits a file using a regex pattern to find text to be replaced by a specified replacement string.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Edit-File [-Path] <String[]> [-Force] [-PassThru] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Edit-File -LiteralPath <String[]> [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Edit-File [-Pattern] <String[]> [-Replacement] <String[]> [-CaseSensitive] [-Encoding <String>] [-SimpleMatch]
 [-SingleString] [<CommonParameters>]
```

## DESCRIPTION
The Edit-File cmdlet modifies the specified files using a search pattern and replacement text.
The search pattern is specified by the Pattern parameter and can be either "simple match" text or a regular expression. 
The replacement text is specified by the Replacement parameter. 
The Edit-File cmdlet can also be used to edit files interactively. 
By default, notepad.exe is used to interactively edit the specified file. 
You can specify an alternate interactive text editor using $Pscx:Preferences\['TextEditor\] = 'notepad2.exe'.
    
By default the regex is applied to the file line by line.
You can use the SingleString parameter to load the entire file into memory as a single string. 
With SingleString, the regex is applied to the entire file at once. 
This enables you to specify a regular expression such as '(?s)(\<PostBuildEvent\>).*?(\</PostBuildEvent\>)' that spans multiple lines. 
The regular expression mode modifier '(?s)' enables Singleline mode which causes the '.' metacharacter to match every character including newline characters. 

One consequence of processing the file using the SingleString parameter is that your regex may have to handle carriage return (\r) characters. 
The regex metacharacter $ matches only newline (\n) and NOT carriage return (\r) characters. 
You need to be aware of this when using the metacharacter $ in Multiline mode to replace the entire contents of a line. 
If you're not careful you can eliminate \r from the newline sequence. 
To avoid this, use an end of line regex positve look-ahead pattern like '(?=\r$)'.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
PS C:\> Edit-File
```

Starts the editor.
Notepad.exe is started unless the PSCX TextEditor preference has been set to another text editor. 
You can specify an alternate text editor using $Pscx:Preferences\['TextEditor\] = 'notepad2.exe'

### EXAMPLE 2
PS C:\\\>

```
PS C:\> Edit-File $profile
```

Starts the text editor passing the specified file to be opened.
Notepad.exe is started unless the PSCX TextEditor preference has been set to another text editor. 
You can specify an alternate text editor using $Pscx:Preferences\['TextEditor\] = 'notepad2.exe'

### EXAMPLE 3
PS C:\\\>

```
PS C:\> Edit-File Acme\Src\Foo\Foo.csproj -Pattern v4\.0 -Replacement v4.5.1
```

Edits the C# project file replacing v4.0 with v4.5.1

### EXAMPLE 4
PS C:\\\>

```
PS C:\> Get-ChildItem Acme\Src\*.csproj -Recurse | Edit-File -Pattern v4.0 -Replacement v4.5.1 -Force -SimpleMatch
```

Edits all of the C# project files replacing v4.0 with v4.5.1 and making them writable with the Force parameter.

By using the SimpleMatch parameter, you can specify a Pattern that is not interpreted as a regular expression.

### EXAMPLE 5
PS C:\\\>

```
PS C:\> Get-ChildItem Acme\Src\*.csproj -Recurse | Edit-File -Pattern v4\.0 -Replacement v4.5.1 -Force -PassThru | Set-ReadOnly
```

Edits all of the C# project files replacing v4.0 with v4.5.1 and making them writable with the Force parameter.

The PassThru switch causes each file to be passed down the pipeline to the Set-ReadOnly command.

### EXAMPLE 6
PS C:\\\>

```
PS C:\> $pattern = '(?s)(<PostBuildEvent>).*?(</PostBuildEvent>)'
 PS C:\> Get-ChildItem Acme\Src\*.csproj -Recurse | Edit-File -Pattern $pattern -Replacement '$1$2' -SingleString
```

Edits all of the C# project files effectivly removing all text between the opening and closing PostBuildEvent XML tags.

Specifying the SingleString parameter loads the file into memory as a single string. 
This enables Singleline mode which causes the '.' metacharacter to match newline (\n) characters. 
This allows a regex pattern to select text that spans multiple lines.

### EXAMPLE 7
PS C:\\\>

```
PS C:\> Edit-File site.css -Pattern '#555\s*;' -Replacement '#5f5f5f;' -Encoding ascii
```

The Encoding parameter specifies that the cmdlet writes the file using the specified encoding.

## PARAMETERS

### -Path
Specifies the path to the file to edit.
Wildcard syntax is allowed.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### -Pattern
Specifies the text to replace.
Type a string or regular expression.
If you type a string, use the SimpleMatch parameter.
To learn about regular expressions, see about_Regular_Expressions.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LiteralPath
Specifies a path to the file to edit.
The value of -LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell Windows PowerShell not to interpret any characters as escape sequences.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Replacement
The replacement string to use for the specified pattern. 
You can use regular expression substitutions in the replacement string.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CaseSensitive
Makes Pattern matches case-sensitive.
By default, Pattern matches are not case-sensitive.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Encoding
Specifies the type of character encoding used to write to the file.
Valid values are "Unicode", "UTF7", "UTF8", "UTF32", "ASCII", "BigEndianUnicode", "Default", and "OEM". 
By default, the cmdlet uses the encoding it detected while reading the file.

"Default" uses the encoding of the system's current ANSI code page.

"OEM" uses the current original equipment manufacturer code page identifier for the operating system.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Allows the cmdlet to edit files that are read-only by making them writable.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Passes a FileInfo object representing the file to the pipeline.
By default, this cmdlet does not generate any output.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SimpleMatch
Uses a simple match rather than a regular expression match.
In a simple match, Edit-File searches the file for the text in the Pattern parameter.
It does not interpret the value of the Pattern parameter as a regular expression statement.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SingleString
Processes the file's contents as a single string. 
By default, the cmdlet processes the file one line at at time. 
Using SingleString enables regex patterns to select text that spans multiple lines. 
In order to take take advantage of SingleString you will likely need to use the Singleline mode modifier (?s), Multiline mode modifier (?m) or both (?sm).

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_3
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

### System.String
## OUTPUTS

### None or a System.IO.FileInfo object representing the file.
## NOTES
*

## RELATED LINKS
