---
external help file: WriteAscii-help.xml
Module Name: WriteAscii
online version:
schema: 2.0.0
---

# Write-Ascii

## SYNOPSIS
Svendsen Tech's PowerShell ASCII art module creates ASCII art characters
from a subset of common letters, numbers and punctuation characters.
You can add new characters by editing the XML (for developers).

MIT license.

Copyright (c) 2012-present, Joakim Borger Svendsen, Svendsen Tech.
All rights reserved.

## SYNTAX

```
Write-Ascii [-InputObject] <String[]> [-PrependChar] [-Compress] [[-ForegroundColor] <String>]
 [[-BackgroundColor] <String>] [<CommonParameters>]
```

## DESCRIPTION
This script reads characters from an XML file that's expected to have the name
"letters.xml", be encoded in UTF-8 and to be in the module's working directory.

It was written to be used in conjunction with a modified version of
PowerBot (http://poshcode.org/2510), a simple IRC bot framework written
using SmartIrc4Net; that's why it can prepend an apostrophe - because somewhere
along the way the leading spaces get lost before it hits the IRC channel.

Currently the XML only contains lowercase letters, mostly because PowerShell/
Windows is case-insensitive by default, which isn't an advantage here.

Example:
PS C:\\\> Import-Module WriteAscii
PS C:\\\> Write-Ascii "ASCII!"
                   _  _  _
  __ _  ___   ___ (_)(_)| |
 / _\` |/ __| / __|| || || |
| (_| |\__ \| (__ | || ||_|
 \__,_||___/ \___||_||_|(_)
PS C:\\\>

## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -InputObject


```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases: InputText

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PrependChar
Optional.
Makes the script prepend an apostrophe.

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

### -Compress


```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: Compression

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForegroundColor
Optional.
Console only.
Changes text foreground color.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: Default
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
Optional.
Console only.
Changes text background color.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: Default
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
