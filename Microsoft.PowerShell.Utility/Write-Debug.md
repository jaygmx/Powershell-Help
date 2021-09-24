---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
Module Name: Microsoft.PowerShell.Utility
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/write-debug?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Write-Debug

## SYNOPSIS
Writes a debug message to the console.

## SYNTAX

```
Write-Debug [-Message] <String> [<CommonParameters>]
```

## DESCRIPTION
The \`Write-Debug\` cmdlet writes debug messages to the host from a script or command.

By default, debug messages are not displayed in the console, but you can display them by using the Debug parameter or the \`$DebugPreference\` variable.

## EXAMPLES

### Example 1: Understand $DebugPreference
```
Write-Debug "Cannot open file."
```

The default value of \`$DebugPreference\` is SilentlyContinue .
Therefore, the message is not displayed in the console.

### Example 2: Change the value of $DebugPreference
```
PS> $DebugPreference
SilentlyContinue
PS> Write-Debug "Cannot open file."
PS>
PS> $DebugPreference = "Continue"
PS> Write-Debug "Cannot open file."
DEBUG: Cannot open file.
```

For more information about \`$DebugPreference\`, see about_Preference_Variables (/powershell/module/Microsoft.PowerShell.Core/About/about_Preference_Variables).

### Example 3: Use the Debug parameter to override $DebugPreference
```
function Test-Debug {
    [CmdletBinding()]
    param()
    Write-Debug ('$DebugPreference is ' + $DebugPreference)
    Write-Host ('$DebugPreference is ' + $DebugPreference)
}

PS> Test-Debug
$DebugPreference is SilentlyContinue

PS> Test-Debug -Debug
DEBUG: $DebugPreference is Continue
$DebugPreference is Continue
PS> $DebugPreference
SilentlyContinue
```

Notice that the value of \`$DebugPreference\` changes when you use the Debug parameter.
This change only affects the scope of the function.
The value is not affected outside the function.

For more information about the Debug common parameter, see about_CommonParameters (https://go.microsoft.com/fwlink/?LinkID=113216).

## PARAMETERS

### -Message
Specifies the debug message to send to the console.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: Msg

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
You can pipe a string that contains a debug message to \`Write-Debug\`.

## OUTPUTS

### None
\`Write-Debug\` only writes to the debug stream.
It does not write any objects to the pipeline.

## NOTES

## RELATED LINKS

[about_Output_Streams]()

[about_Redirection]()

[Write-Error]()

[Write-Host]()

[Write-Output]()

[Write-Progress]()

[Write-Verbose]()

[Write-Warning]()

