---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Get-PSOneToken.ps1
schema: 2.0.0
---

# Group-ObjectFast

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### Analysis (Default)
```
Group-ObjectFast -Property <String[]> [-NoElement] -InputObject <Object> [<CommonParameters>]
```

### Separation
```
Group-ObjectFast -Property <String[]> [-AsHashtable] [-AsString] -InputObject <Object> [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -AsHashtable
{{ Fill AsHashtable Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Separation
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AsString
{{ Fill AsString Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Separation
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
{{ Fill InputObject Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NoElement
{{ Fill NoElement Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Analysis
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
{{ Fill Property Description }}

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Object

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
