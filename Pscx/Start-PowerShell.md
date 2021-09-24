---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# Start-PowerShell

## SYNOPSIS
Starts a new Windows PowerShell process.

## SYNTAX

```
Start-PowerShell [[-Version] <Double>] [-Architecture <String>] [-Command <Object>]
 [-Credential <PSCredential>] [-WorkingDirectory <String>] [-Wait] [-PSConsoleFile <String>]
 [-ExecutionPolicy <ExecutionPolicy>] [-File <String>] [-EncodedCommand <String>] [-InputFormat <String>]
 [-OutputFormat <String>] [-WindowStyle <String>] [-NoExit] [-NoLogo] [-NoProfile] [-NoNewWindow]
 [-NonInteractive] [-Mta] [-Sta] [-Arguments <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Starts a new Windows PowerShell process using PowerShell's parameter
parsing engine to parse the parameters for the PowerShell executable.
This command exposes a few of the Start-Process commands it uses such as
-Wait, -Credential and -WorkingDirectory. 
Note: If -NoNewWindow is
specified, PowerShell is invoked using the call operator (&) instead of
with the Start-Process cmdlet.

## EXAMPLES

### EXAMPLE 1
```
Start-PowerShell -NoProfile -NoExit -File $pwd\foo.ps1
```

### EXAMPLE 2
```
Start-PowerShell -NoProfile -NoLogo -Credential (Get-Credential)
```

### EXAMPLE 3
```
Start-PowerShell -NoProfile -NoNewWindow -File $pwd\foo.ps1
```

### EXAMPLE 4
```
Start-PowerShell -Architecture x64 -NoNewWindow -Command {[IntPtr]::Size}
```

### EXAMPLE 5
```
Start-PowerShell -Architecture x86 -NoNewWindow -Command {[IntPtr]::Size}
```

## PARAMETERS

### -Version
Starts the specified version of Windows PowerShell.
Enter a version number with the parameter, such as "-version 2.0".

```yaml
Type: System.Double
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Architecture
Starts PowerShell with the desired architecture: x86, x64 or same
architecture as the launching PowerShell process.
Valid values are: x86, x64 and Same.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Command
Executes the specified commands (and any parameters) as though they were
typed at the Windows PowerShell command prompt, and then exits, unless
NoExit is specified.
The value of Command can be "-", a string.
or a
script block.

If the value of Command is "-", the command text is read from standard
input.

If the value of Command is a script block, the script block must be enclosed
in braces ({}).
You can specify a script block only when running PowerShell.exe
in Windows PowerShell.
The results of the script block are returned to the
parent shell as deserialized XML objects, not live objects.

If the value of Command is a string, Command must be the last parameter
in the command , because any characters typed after the command are
interpreted as the command arguments.

To write a string that runs a Windows PowerShell command, use the format:
"& {\<command\>}"
where the quotation marks indicate a string and the invoke operator (&)
causes the command to be executed.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
Specifies a user account that has permission to perform this action.
Type
a user-name, such as "User01" or "Domain01\User01", or enter a
PSCredential object, such as one from the Get-Credential cmdlet.
By
default, the cmdlet uses the credentials of the current user.
This parameter can't be used in conjunction with the NoNewWindow parameter.

```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WorkingDirectory
Specifies the location of the executable file or document that runs in the
process. 
The default is the current directory.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Wait
Waits for the specified process to complete before accepting more input.
This parameter suppresses the command prompt or retains the window until
the process completes.

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

### -PSConsoleFile
Loads the specified Windows PowerShell console file.
To create a console
file, use Export-Console in Windows PowerShell.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExecutionPolicy
Sets the default execution policy for the current session and saves it
in the $env:PSExecutionPolicyPreference environment variable.
This parameter does not change the Windows PowerShell execution policy
that is set in the registry.

```yaml
Type: Microsoft.PowerShell.ExecutionPolicy
Parameter Sets: (All)
Aliases:
Accepted values: Unrestricted, RemoteSigned, AllSigned, Restricted, Default, Bypass, Undefined

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -File
Runs the specified script in the local scope ("dot-sourced"), so that the
functions and variables that the script creates are available in the
current session.
Enter the script file path and any parameters.
File must be the last parameter in the command, because all characters
typed after the File parameter name are interpreted
as the script file path followed by the script parameters.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: PSPath

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EncodedCommand
Accepts a base-64-encoded string version of a command.
Use this parameter
to submit commands to Windows PowerShell that require complex quotation
marks or curly braces.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputFormat
Describes the format of data sent to Windows PowerShell.
Valid values are
"Text" (text strings) or "XML" (serialized CLIXML format).

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputFormat
Determines how output from Windows PowerShell is formatted.
Valid values
are "Text" (text strings) or "XML" (serialized CLIXML format).

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WindowStyle
Sets the window style to Normal, Minimized, Maximized or Hidden.
This parameter can't be used in conjunction with the NoNewWindow parameter.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoExit
Does not exit after running startup commands.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: NE

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoLogo
Hides the copyright banner at startup.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: NL

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoProfile
Does not load the Windows PowerShell profile.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: NP

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoNewWindow
Uses the call invocation operator to start PowerShell instead of Start-Process.
This parameter can't be used in conjunction with the WindowStyle parameter.

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

### -NonInteractive
Does not present an interactive prompt to the user.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: NI

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Mta
Start the shell using a multithreaded apartment.

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

### -Sta
Starts the shell using a single-threaded apartment.
Single-threaded apartment (STA) is the default.

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

### -Arguments


```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
