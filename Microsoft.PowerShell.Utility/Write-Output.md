---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
Module Name: Microsoft.PowerShell.Utility
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/write-output?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Write-Output

## SYNOPSIS
Writes the specified objects to the pipeline.
If \`Write-Output\` is the last command in the pipeline, the objects are displayed in the console.

## SYNTAX

```
Write-Output [-InputObject] <PSObject> [-NoEnumerate] [<CommonParameters>]
```

## DESCRIPTION
Writes the specified objects to the pipeline.
If \`Write-Output\` is the last command in the pipeline, the objects are displayed in the console.

\`Write-Output\` sends objects to the primary pipeline, also known as the "output stream" or the "success pipeline." To send error objects to the error pipeline, use \`Write-Error\`.

This cmdlet is typically used in scripts to display strings and other objects on the console.
One of the built-in aliases for \`Write-Output\` is \`echo\` and similar to other shells that use \`echo\`.
The default behavior is to display the output at the end of a pipeline.
In PowerShell, it is generally not necessary to use the cmdlet in instances where the output is displayed by default.
For example, \`Get-Process | Write-Output\` is equivalent to \`Get-Process\`.
Or, \`echo "Home directory: $HOME"\` can be written, \`"Home directory: $HOME"\`.

By default, \`Write-Output\` enumerates through collection objects.
However, \`Write-Output\` can also be used to pass collections down the pipeline as a single object with the NoEnumerate parameter.

## EXAMPLES

### Example 1: Get objects and write them to the console
```
$P = Get-Process
Write-Output $P
```

### Example 2: Pass output to another cmdlet
```
Write-Output "test output" | Get-Member
```

### Example 3: Suppress enumeration in output
```
Write-Output 1,2,3 | Measure-Object

Count    : 3
...

Write-Output 1,2,3 -NoEnumerate | Measure-Object

Count    : 1
...
```

## PARAMETERS

### -InputObject
Specifies the objects to send down the pipeline.
Enter a variable that contains the objects, or type a command or expression that gets the objects.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NoEnumerate
By default, the \`Write-Output\` cmdlet always enumerates its output.
The NoEnumerate parameter suppresses the default behavior, and prevents \`Write-Output\` from enumerating output.
The NoEnumerate parameter has no effect if the command is wrapped in parentheses, because the parentheses force enumeration.
For example, \`(Write-Output 1,2,3)\` still enumerates the array.

The NoEnumerate parameter is only useful within a pipeline.
Trying to see the effects of NoEnumerate in the console is problematic because PowerShell adds \`Out-Default\` to the end of every command line, which results in enumeration.
But if you pipe \`Write-Output -NoEnumerate\` to another cmdlet, the downstream cmdlet receives the collection object, not the enumerated items of the collection.

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

### System.Management.Automation.PSObject
You can pipe objects to \`Write-Output\`.

## OUTPUTS

### System.Management.Automation.PSObject
\`Write-Output\` returns the objects that are submitted as input.

## NOTES

## RELATED LINKS

[about_Output_Streams]()

[about_Redirection]()

[Tee-Object]()

[Write-Debug]()

[Write-Error]()

[Write-Host]()

[Write-Information]()

[Write-Progress]()

[Write-Verbose]()

[Write-Warning]()

