---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Write-PscxClipboard

## SYNOPSIS
PSCX Cmdlet: Writes objects to the clipboard using their string representation, bypassing the default PowerShell formatting.

## SYNTAX

```
Write-PscxClipboard [-Object] <Object> [-Separator <Object>] [-NoNewLine] [<CommonParameters>]
```

## DESCRIPTION
Writes objects to the clipboard using their string representation, bypassing the default PowerShell formatting.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Object
Accepts an object as input to the cmdlet.
Enter a variable that contains the objects or type a command or expression that gets the objects.

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

### -NoNewLine
Specifies that the content written to the clipboard does not end with a newline character.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Separator
String to output between objects written to the clipboard.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: One space
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-PscxClipboard]()

[Out-PscxClipboard]()

[Set-PscxClipboard]()

