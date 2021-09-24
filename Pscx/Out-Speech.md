---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Out-Speech

## SYNOPSIS
Outputs text as spoken words.

## SYNTAX

```
Out-Speech [-InputObject] <PSObject[]> [-Wait] [-Purge] [-ReadFiles] [-ReadXml] [-NotXml] [<CommonParameters>]
```

## DESCRIPTION
Outputs text as spoken words.

## EXAMPLES

### EXAMPLE 1
```
Out-Speech "Hello World"
Speaks "hello world".
```

### EXAMPLE 2
```
Get-Content quotes.txt | Get-Random | Out-Speech -wait
Speaks a random quote from a file.
```

### EXAMPLE 3
```
Out-Speech -readfiles "Hitchhiker's Guide To The Galaxy.txt"
Speaks the entire contents of a file.
```

## PARAMETERS

### -InputObject
One or more objects to speak.

```yaml
Type: System.Management.Automation.PSObject[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Wait
Wait for the machine to read each item (NOT asynchronous).

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

### -Purge
Purge all other speech requests before making this call.

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

### -ReadFiles
Read the contents of the text files indicated.

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

### -ReadXml
Treat input as speech XML markup.

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

### -NotXml
Do NOT parse as XML (if text starts with "\<" but is not XML).

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Joel "Jaykul" Bennett

## RELATED LINKS
