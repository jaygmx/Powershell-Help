---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-ScreenHtml

## SYNOPSIS
Functions to generate HTML "screen shot" of the host buffer.

## SYNTAX

```
Get-ScreenHtml [[-Count] <Object>]
```

## DESCRIPTION
Functions to generate HTML "screen shot" of the host buffer.

## EXAMPLES

### EXAMPLE 1
```
Get-ScreenHtml > screen.html
Generates an HTML representation of the host's screen buffer and saves it to file.
```

### EXAMPLE 2
```
Get-ScreenHtml 25 > screen.html
Generates an HTML representation of the first 25 lines of the host's screen buffer and saves it to file.
```

## PARAMETERS

### -Count
The number of lines of the host buffer to create a screen shot from.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: $Host.UI.RawUI.WindowSize.Height
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
Author: Jachym Kouba

## RELATED LINKS
