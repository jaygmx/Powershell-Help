---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Invoke-NullCoalescing

## SYNOPSIS
Similar to the C# ??
operator e.g.
name = value ??
String.Empty

## SYNTAX

```
Invoke-NullCoalescing [-PrimaryExpr] <ScriptBlock> [-AlternateExpr] <ScriptBlock> [-InputObject <PSObject>]
 [<CommonParameters>]
```

## DESCRIPTION
Similar to the C# ??
operator e.g.
name = value ??
String.Empty;
where value would be a Nullable&lt;T&gt; in C#. 
Even though PowerShell
doesn't support nullables yet we can approximate this behavior.
In the example below, $LogDir will be assigned the value of $env:LogDir
if it exists and it's not null, otherwise it get's assigned the
result of the second script block (C:\Windows\System32\LogFiles).
This behavior is also analogous to Korn shell assignments of this form:
LogDir = ${$LogDir:-$WinDir/System32/LogFiles}

## EXAMPLES

### EXAMPLE 1
```
$LogDir = ?? {$env:LogDir} {"$env:windir\System32\LogFiles"}
$LogDir is set to the value of $env:LogDir unless it doesn't exist, in which case it
will then default to "$env:windir\System32\LogFiles".
```

## PARAMETERS

### -PrimaryExpr
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

### -AlternateExpr
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

### -InputObject
Specifies the input object.
Invoke-NullCoalescing injects the InputObject into each
scriptblock provided via the PrimaryExpr and AlternateExpr parameters.

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
Aliases:  ??
Author:   Keith Hill

## RELATED LINKS
