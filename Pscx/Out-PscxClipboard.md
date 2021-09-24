---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Out-PscxClipboard

## SYNOPSIS
PSCX Cmdlet: Formats text via Out-String before placing in clipboard.
Can also place string in clipboard as a file.

## SYNTAX

### Text (Default)
```
Out-PscxClipboard [-InputObject] <PSObject> [-Width <Int32>] [-NoTrimEnd] [<CommonParameters>]
```

### VirtualFile
```
Out-PscxClipboard [-InputObject] <PSObject> [-Width <Int32>] [-NoTrimEnd] [-AsFile] [[-PasteFileName] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Formats text via Out-String before placing in clipboard.
Can also place string in clipboard as a file.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -InputObject
Accepts an object as input to the cmdlet.
Enter a variable that contains the objects or type a command or expression that gets the objects.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PasteFileName
If AsFile switch is set, value supplied will be the name of the file placed in the clipboard.

```yaml
Type: System.String
Parameter Sets: VirtualFile
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AsFile
Copies input as string and places on clipboard as a file.
If PasteFileName is not supplied, the file will be named randomly with a .txt extension.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: VirtualFile
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoTrimEnd
Suppresses trimming whitespace from the line of each line of input.

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

### -Width
Specifies the number of characters in each line of output.
Any additional characters are truncated, not wrapped.
If you omit this parameter, the width is determined by the characteristics of the host.
The default for the PowerShell.exe host is 120 (characters).

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Same as Out-String -Width Default.
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

[Set-PscxClipboard]()

[Write-PscxClipboard]()

