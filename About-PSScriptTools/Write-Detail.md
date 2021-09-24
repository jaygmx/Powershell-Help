---
external help file: PSScriptTools-help.xml
Module Name:
online version: http://bit.ly/31UuI26
schema: 2.0.0
---

# Write-Detail

## SYNOPSIS
Write a detailed message string.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Write-Detail [[-Message] <String>] [-Prefix <String>] [-Date] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Write-Detail [[-Message] <String>] [-Prefix <String>] [-Time] [<CommonParameters>]
```

## DESCRIPTION
This command is designed to be used within your functions and scripts to make it easier to write a detailed message that you can use as verbose output.
The assumption is that you are using an advanced function with Begin, Process, and End scriptblocks.
You can create a detailed message to indicate what part of the code is being executed.
The output can include a full-time stamp, or a time string which includes a millisecond value.

In a script you might use it like this in a Begin block:

$pfx = "BEGIN"

Write-Detail "Starting $($MyInvocation.MyCommand)" -Prefix $pfx | Write-Verbose

Write-Detail "PS $($PSVersiontable.PSVersion)" -Prefix $pfx | Write-Verbose

If you don't specify a prefix, it will default to PROCESS.

## EXAMPLES

### EXAMPLE 1
```
PS C:\> Write-Detail "Getting file information" -Prefix Process
[PROCESS] Getting file information
```

Normally you would use this command in a function, but here is an example from the console so that you can see what to expect.

## PARAMETERS

### -Message
The message to display after the time stamp and prefix.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Prefix
Indicate whether you are in the BEGIN, PROCESS, or END script block.
Although you can specify any text.
It will be displayed in upper case.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: PROCESS
Accept pipeline input: False
Accept wildcard characters: False
```

### -Date
Display a date value like 9/15/2020 11:36:41.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Time
Display a time value with milliseconds like 11:37:01:4029.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

### None
## OUTPUTS

### System.String
## NOTES
* Learn more about PowerShell: http://jdhitsolutions.com/blog/essential-powershell-resources/

## RELATED LINKS

[Write-Verbose]()

