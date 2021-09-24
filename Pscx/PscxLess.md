---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# PscxLess

## SYNOPSIS
PscxLess provides better paging of output from cmdlets.

## SYNTAX

```
PscxLess [[-Path] <String[]>] [[-LiteralPath] <String[]>]
```

## DESCRIPTION
PscxLess provides better paging of output from cmdlets.
By default PowerShell uses more.com for paging which is a pretty minimal paging app that doesn't support advanced
navigation features. 
This function uses Less.exe ie Less394 as the replacement for more.com. 
Less can navigate
down as well as up and can be scrolled by page or by line and responds to the Home and End keys.
Less also
supports searching the text by pressing the "/" key followed by the term to search for then the "Enter" key.
One of the primary keyboard shortcuts to know with less.exe is the key to exit.
Pressing the "q" key will exit
less.exe. 
For more help on less.exe press the "h" key. 
If you prefer to use more.com set the PSCX preference
variable PageHelpUsingLess to $false e.g.
$Pscx:Preferences\['PageHelpUsingLess'\] = $false

## EXAMPLES

### EXAMPLE 1
```
man about_profiles -full
This sends the help output of the about_profiles topic to the help function which pages the output.
Man is an alias for the "help" function. PSCX overrides the help function to page help using either
the built-in PowerShell "more" function or the PSCX "less" function depending on the value of the
PageHelpUsingLess preference variable.
```

### EXAMPLE 2
```
PscxLess *.txt
Opens each text file in less.exe in succession.  Pressing ':n' moves to the next file.
```

## PARAMETERS

### -Path
The path to the file to view. 
Wildcards are accepted.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LiteralPath
Specifies the path to a file to view.
Unlike Path, the value of LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in
single quotation marks.
Single quotation marks tell Windows PowerShell not to interpret any characters
as escape sequences.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
This function is just a passthru in all other hosts except for the PowerShell.exe console host.

## RELATED LINKS

[http://en.wikipedia.org/wiki/Less_(Unix)](http://en.wikipedia.org/wiki/Less_(Unix))

