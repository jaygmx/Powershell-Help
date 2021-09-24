---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/tricks/performance/pipeline
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.2/Foreach-ObjectFast.ps1
schema: 2.0.0
---

# Foreach-ObjectFast

## SYNOPSIS
Faster Foreach-Object

## SYNTAX

```
Foreach-ObjectFast [[-Process] <ScriptBlock>] [[-Begin] <ScriptBlock>] [[-End] <ScriptBlock>]
```

## DESCRIPTION
Foreach-ObjectFast can replace the built-in Foreach-Object and improves pipeline speed considerably.
Foreach-ObjectFast supports only the most commonly used parameters -Begin, -Process, and -End, so you can replace

1..100 | Foreach-Object { 'Server{0:d3}' -f $_ }

with

1..100 | Foreach-ObjectFast { 'Server{0:d3}' -f $_ }

but you cannot currently replace instances of Foreach-Object that uses the less commonly used parameters, 
like -RemainingScripts, -MemberNames, and -ArgumentList

Foreach-ObjectFast has a performance benefit per iteration, so the more objects
you send through the pipeline, the more significant performace benefits you will see.

Foreach-ObjectFast is using a steppable pipeline internally which performs better.
However because of this, the debugging experience will be different, and internal
variables such as $MyInvocation may yield different results.
For most every-day tasks,
these changes are not important.

A complete explanation of what Where-ObjectFast does can be found here:
https://powershell.one/tricks/performance/pipeline

## EXAMPLES

### EXAMPLE 1
```
$stopwatch = [System.Diagnostics.Stopwatch]::StartNew()
```

$result = 1..1000000 | Foreach-ObjectFast -Process {
  "I am at $_"
}

$report = '{0} elements in {1:n2} seconds' 
$report -f $result.Count, $stopwatch.Elapsed.TotalSeconds 

Demos the speed improvements.
Run this script to see how well it performs,
then replace Foreach-ObjectFast with the default Foreach-Object, and check out
the performace difference.
$result is the same in both cases.

## PARAMETERS

### -Process
executes for each pipeline element

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Begin
executes once before the pipeline is started.
can be used for initialization routines

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -End
executes once after all pipeline elements have been processed
can be used to do cleanup work

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one/tricks/performance/pipeline
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.2/Foreach-ObjectFast.ps1](https://powershell.one/tricks/performance/pipeline
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.2/Foreach-ObjectFast.ps1)

[https://powershell.one/tricks/performance/pipeline
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.2/Foreach-ObjectFast.ps1]()

