---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Invoke-Ternary

## SYNOPSIS
Similar to the C# ?
: operator e.g.
name = (value != null) ?
String.Empty : value

## SYNTAX

```
Invoke-Ternary [-Condition] <ScriptBlock> [-TrueBlock] <ScriptBlock> [-FalseBlock] <ScriptBlock>
 [-InputObject <PSObject>] [<CommonParameters>]
```

## DESCRIPTION
Similar to the C# ?
: operator e.g.
name = (value != null) ?
String.Empty : value.
The first script block is tested.
If it evaluates to $true then the second scripblock
is evaluated and its results are returned otherwise the third scriptblock is evaluated
and its results are returned.

## EXAMPLES

### EXAMPLE 1
```
$toolPath = ?: {[IntPtr]::Size -eq 4} {"$env:ProgramFiles(x86)\Tools"} {"$env:ProgramFiles\Tools"}}
Each input number is evaluated to see if it is > 5.  If it is then "Greater than 5" is
displayed otherwise "Less than or equal to 5" is displayed.
```

### EXAMPLE 2
```
1..10 | ?: {$_ -gt 5} {"Greater than 5";$_} {"Less than or equal to 5";$_}
Each input number is evaluated to see if it is > 5.  If it is then "Greater than 5" is
displayed otherwise "Less than or equal to 5" is displayed.
```

## PARAMETERS

### -Condition
The condition that determines whether the TrueBlock scriptblock is used or the FalseBlock
is used.

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TrueBlock
This block gets evaluated and its contents are returned from the function if the Conditon
scriptblock evaluates to $true.

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FalseBlock
This block gets evaluated and its contents are returned from the function if the Conditon
scriptblock evaluates to $false.

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Specifies the input object.
Invoke-Ternary injects the InputObject into each scriptblock
provided via the Condition, TrueBlock and FalseBlock parameters.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Aliases:  ?:
Author:   Karl Prosser

## RELATED LINKS
