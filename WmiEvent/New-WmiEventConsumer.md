---
external help file: WmiEvent-Help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# New-WmiEventConsumer

## SYNOPSIS

## SYNTAX

### SMTPComputerSet
```
New-WmiEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [<CommonParameters>]
```

### NtEventLogComputerSet
```
New-WmiEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-Category <UInt16>] -EventID <UInt32> [-EventType <UInt32>]
 [-InsertionStringTemplates <String[]>] -NameOfUserSidProperty <String> -NameOfRawDataProperty <String>
 -SourceName <String> [-UNCServerName <String>] [<CommonParameters>]
```

### LogFileComputerSet
```
New-WmiEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] -Filename <String> [-IsUnicode <Boolean>] [-MaximumFileSize <UInt64>] -Text <String>
 [<CommonParameters>]
```

### CommandLineTemplateComputerSet
```
New-WmiEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>] -CommandLineTemplate <String>
 [-CreateNewProcessGroup <Boolean>] [-CreateSeparateWowVdm <Boolean>] [-CreateSharedWowVdm <Boolean>]
 [-ForceOffFeedback <Boolean>] [-ForceOnFeedback <Boolean>] [-Priority <Int32>] [-RunInteractively <Boolean>]
 [-ShowWindowCommand <UInt32>] [-UseDefaultErrorMode <Boolean>] [-WindowTitle <String>]
 [-WorkingDirectory <String>] [-XCoordinate <UInt32>] [-XNumCharacters <UInt32>] [-XSize <UInt32>]
 [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>] [-YSize <UInt32>] [<CommonParameters>]
```

### CommandLineComputerSet
```
New-WmiEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>] -ExecutablePath <String> [-CreateNewProcessGroup <Boolean>]
 [-CreateSeparateWowVdm <Boolean>] [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>]
 [-ForceOnFeedback <Boolean>] [-Priority <Int32>] [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>]
 [-UseDefaultErrorMode <Boolean>] [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>]
 [-XNumCharacters <UInt32>] [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>]
 [-YSize <UInt32>] [<CommonParameters>]
```

### ActiveScriptTextComputerSet
```
New-WmiEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>] -ScriptingEngine <String> -ScriptText <String>
 [<CommonParameters>]
```

### ActiveScriptFileComputerSet
```
New-WmiEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>] -ScriptingEngine <String> -ScriptFileName <String>
 [<CommonParameters>]
```

### SMTPSessionSet
```
New-WmiEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] [<CommonParameters>]
```

### NtEventLogSessionSet
```
New-WmiEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] [-Category <UInt16>]
 -EventID <UInt32> [-EventType <UInt32>] [-InsertionStringTemplates <String[]>] -NameOfUserSidProperty <String>
 -NameOfRawDataProperty <String> -SourceName <String> [-UNCServerName <String>] [<CommonParameters>]
```

### LogFileSessionSet
```
New-WmiEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] -Filename <String>
 [-IsUnicode <Boolean>] [-MaximumFileSize <UInt64>] -Text <String> [<CommonParameters>]
```

### CommandLineTemplateSessionSet
```
New-WmiEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>]
 -CommandLineTemplate <String> [-CreateNewProcessGroup <Boolean>] [-CreateSeparateWowVdm <Boolean>]
 [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>] [-ForceOnFeedback <Boolean>] [-Priority <Int32>]
 [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>] [-UseDefaultErrorMode <Boolean>]
 [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>] [-XNumCharacters <UInt32>]
 [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>] [-YSize <UInt32>] [<CommonParameters>]
```

### CommandLineSessionSet
```
New-WmiEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>]
 -ExecutablePath <String> [-CreateNewProcessGroup <Boolean>] [-CreateSeparateWowVdm <Boolean>]
 [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>] [-ForceOnFeedback <Boolean>] [-Priority <Int32>]
 [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>] [-UseDefaultErrorMode <Boolean>]
 [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>] [-XNumCharacters <UInt32>]
 [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>] [-YSize <UInt32>] [<CommonParameters>]
```

### ActiveScriptTextSessionSet
```
New-WmiEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>]
 -ScriptingEngine <String> -ScriptText <String> [<CommonParameters>]
```

### ActiveScriptFileSessionSet
```
New-WmiEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>]
 -ScriptingEngine <String> -ScriptFileName <String> [<CommonParameters>]
```

### SmtpSessionSet
```
New-WmiEventConsumer -Name <String> [-ThrottleLimit <Int32>] [-BccLine <String>] [-CcLine <String>]
 [-FromLine <String>] [-HeaderFields <String[]>] -Message <String> [-ReplyToLine <String>] -SMTPServer <String>
 [-Subject <String>] -ToLine <String> [<CommonParameters>]
```

### SmtpComputerSet
```
New-WmiEventConsumer -Name <String> [-ThrottleLimit <Int32>] [-BccLine <String>] [-CcLine <String>]
 [-FromLine <String>] [-HeaderFields <String[]>] -Message <String> [-ReplyToLine <String>] -SMTPServer <String>
 [-Subject <String>] -ToLine <String> [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```
Add-WmiEventConsumer -ComputerName WORKSTATION1 -ConsumerFile AS_ExtrinsicHTTPPOST
```

### EXAMPLE 2
```
Add-WmiEventConsumer -ComputerName SERVER1 -Name LogTest -Filename C:\temp\output.txt -Text "%TargetInstance%"


Path          : \\SERVER1\root\subscription:LogFileEventConsumer.Name="LogTest"
RelativePath  : LogFileEventConsumer.Name="LogTest"
Server        : localhost
NamespacePath : root\subscription
ClassName     : LogFileEventConsumer
IsClass       : False
IsInstance    : True
IsSingleton   : False
```

Add a LogFile Event Consumer named LogTest on SERVER1 that outputs to C:\temp\output.txt

### EXAMPLE 3
```
Add-WMIEventConsumer -Name commandlineexe -ExecutablePath calc.exe


Path          : \\localhost\root\subscription:CommandLineEventConsumer.Name="commandlineexe
RelativePath  : CommandLineEventConsumer.Name="commandlineexe"
Server        : localhost
NamespacePath : root\subscription
ClassName     : CommandLineEventConsumer
IsClass       : False
IsInstance    : True
IsSingleton   : False
```

Adds a CommandLineEventConsumer that starts a calc.exe process in the background

## PARAMETERS

### -ComputerName
Adds an Event Consumer running on the specified computers.
The default is the local computer.

Type the NetBIOS name, an IP address, or a fully qualified domain name of one or more computers.
To specify the local computer, type the computer name, a dot (.), or "localhost".

This parameter does not rely on Windows PowerShell remoting.
You can use the ComputerName parameter of Add-WmiEventConsumer even if your computer is not configured to run remote commands.

```yaml
Type: System.String[]
Parameter Sets: SMTPComputerSet, NtEventLogComputerSet, LogFileComputerSet, CommandLineTemplateComputerSet, CommandLineComputerSet, ActiveScriptTextComputerSet, ActiveScriptFileComputerSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Unique identifier for the event consumer.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BccLine
A list of addresses, separated by a comma or semicolon, in the format of a standard string template to which the message is sent as a blind carbon copy.

```yaml
Type: System.String
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CcLine
A list of addresses, separated by a comma or semicolon, in the format of a standard string template to which the message is sent as a carbon copy.

```yaml
Type: System.String
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FromLine
From line of an email message in the format of a standard string template.
If NULL, a From line is constructed in the form of WinMgmt@MachineName.

```yaml
Type: System.String
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeaderFields
Array of header fields that are inserted into an email message without interpretation.

```yaml
Type: System.String[]
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Message
Standard string template that contains the body of an email message.

```yaml
Type: System.String
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplyToLine
Reply-to line of an email message in the format of a standard string template.
If NULL, no Reply-to line is used.

```yaml
Type: System.String
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SMTPServer
Name of the SMTP server through which an email is sent.
Permissible names are an IP address, or a DNS or NetBIOS name.
This property cannot be NULL.

```yaml
Type: System.String
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
Standard string template that contains the subject of an email message.

```yaml
Type: System.String
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ToLine
A list of addresses, separated by a comma or semicolon, in the format of a standard string template that identifies where the message is to be sent.

```yaml
Type: System.String
Parameter Sets: SmtpSessionSet, SmtpComputerSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Category
Event category.
This is source-specific information and can have any value.

```yaml
Type: System.UInt16
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EventID
Event message in the message DLL.
This property cannot be NULL.

```yaml
Type: System.UInt32
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EventType
Type of event.

```yaml
Type: System.UInt32
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InsertionStringTemplates
Array of standard string templates that is used as the insertion string for an event log record.

```yaml
Type: System.String[]
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NameOfUserSidProperty
Name of the event property that contains a security identifier (SID) to be passed to the ReportEvent function lpUserSid parameter.
The property must be either an array of bytes (uint8) or a string.
If it is an array of bytes, it is assumed to be a SID.
If it is a string, it is a string SID that is converted into a SID.

```yaml
Type: System.String
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NameOfRawDataProperty
Name of the event property that contains data to be passed to the ReportEvent function lpRawData parameter.

```yaml
Type: System.String
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceName
Source name where a message is located.
The customer is assumed to have registered a DLL with the necessary messages.

Note: The value of this parameter must not include a colon (:) character.

```yaml
Type: System.String
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UNCServerName
Name of the computer on which to log an event, or NULL if the event is to be logged on a local server.

Windows Server 2003 with SP1 and Windows Vista:  Authenticated users cannot, by default, log events to the Application log on a remote computer.
As a result, using this property to specify a remote computer will not work.

```yaml
Type: System.String
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filename
Name of a file that includes the path to which the log entries are appended.
If the file does not exist, LogFileEventConsumer attempts to create it. 

The consumer fails when the path does not exist, or when the user who creates the consumer does not have write permissions for the file or path.

```yaml
Type: System.String
Parameter Sets: LogFileComputerSet, LogFileSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsUnicode
If TRUE, the log file is a Unicode text file.
If FALSE, the log file is a multibyte code text file.
If the file exists, this property is ignored and the current file setting is used.
For example, if IsUnicode is FALSE, but the existing file is a Unicode file, then Unicode is used.
If IsUnicode is TRUE, but the file is multibyte code, then multibyte code is used.

```yaml
Type: System.Boolean
Parameter Sets: LogFileComputerSet, LogFileSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaximumFileSize
Maximum size of a log file-in bytes.
If the primary file exceeds its maximum size, the contents are moved to a different file and the primary file is emptied.
A value of 0 (zero) means there is no size limit. 

The default value is 65,535 bytes.
The size of the file is checked before a write operation.
Therefore, you can have a file that is slightly larger than the specified size limit.
The next write operation catches it and starts a new file.

```yaml
Type: System.UInt64
Parameter Sets: LogFileComputerSet, LogFileSessionSet
Aliases:

Required: False
Position: Named
Default value: 65,535
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text
Standard string template for the text of a log entry.

```yaml
Type: System.String
Parameter Sets: LogFileComputerSet, LogFileSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -KillTimeout
Number, in seconds, that the script is allowed to run.
If 0 (zero), which is the default, the script is not terminated.

```yaml
Type: System.UInt32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, ActiveScriptTextComputerSet, ActiveScriptFileComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet, ActiveScriptTextSessionSet, ActiveScriptFileSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommandLineTemplate
Standard string template that specifies the process to be started.
This property can be NULL, and the ExecutablePath property is used as the command line.

```yaml
Type: System.String
Parameter Sets: CommandLineTemplateComputerSet, CommandLineTemplateSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreateNewProcessGroup
If True, the new process is the root process of a new process group.
The process group includes all processes that are descendants of this root process. 

The process identifier of the new process group is the same as this process identifier.
Process groups are used by the GenerateConsoleCtrlEvent method to enable sending a CTRL+C or CTRL+BREAK signal to a group of console processes.

```yaml
Type: System.Boolean
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreateSeparateWowVdm
If True, the new process runs in a private Virtual DOS Machine (VDM).
This is only valid when starting an application running on a 16-bit Windows operating system. 

If set to False, all applications running on a 16-bit Windows operating system run as threads in a single, shared VDM.
For more information, see the Remarks section of this topic.

```yaml
Type: System.Boolean
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreateSharedWowVdm
If True, the CreateProcess method runs the new process in the shared Virtual DOS Machine (VDM).
This property can override the DefaultSeparateVDM switch in the Windows section of Win.ini if set to True.

```yaml
Type: System.Boolean
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExecutablePath
Module to execute.
The string can specify the full path and file name of the module to execute, or it can specify a partial name.
If a partial name is specified, the current drive and current directory are assumed.

The ExecutablePath property can be NULL.
In that case, the module name must be the first white space-delimited token in the CommandLineTemplate property value.
If using a long file name that contains a space, use quoted strings to indicate where the file name ends and the arguments begin-to clarify the file name.

Note: Because the CommandLineTemplate property can be a template where the module to execute is supplied by a variable, a NULL ExecutablePath property permits the module that is specified in the parameter to execute, and then it is out of your control.
Always set the ExecutablePath property in the CommandLineEventConsumer registration to include the required executable, which avoids overwriting by events parameters.
If you must use a template and variable to specify the module to execute, be careful about who is granted full write privilege in the namespace.

```yaml
Type: System.String
Parameter Sets: CommandLineComputerSet, CommandLineSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceOffFeedback
If True, the feedback cursor is forced off while the process is starting.
The normal cursor is displayed.

```yaml
Type: System.Boolean
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceOnFeedback
If True, the cursor is in feedback mode for two seconds after CreateProcess is called.
During those two seconds, if the process makes the first GUI call, the system gives five more seconds to the process.
During those five seconds, if the process shows a window, the system gives another five seconds to the process to finish drawing the window.

```yaml
Type: System.Boolean
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Priority
Scheduling priority level of the process threads.

```yaml
Type: System.Int32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RunInteractively
If True, the process is launched in the interactive WinStation.
If False, the process is launched in the default service WinStation.
This property overrides the DesktopName property.
This property is only used locally, and only if the interactive user is the same user who set up the consumer.

Starting with Windows Vista, the process running the CommandLineEventConsumer instance is started under the LocalSystem account and is in session 0.
Services which run in session 0 cannot interact with user sessions.

Windows Server 2003: If the user logon is through a terminal services connection, the CommandLineEventConsumer process does not run interactively.

```yaml
Type: System.Boolean
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShowWindowCommand
Window show state.

```yaml
Type: System.UInt32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseDefaultErrorMode
If True, the default error mode is used.

```yaml
Type: System.Boolean
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WindowTitle
Title that appears on the title bar of the process.
This property is ignored for GUI applications.

```yaml
Type: System.String
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WorkingDirectory
Working directory for this process.

```yaml
Type: System.String
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -XCoordinate
X-offset, in pixels, from the left edge of the screen to the left edge of the window, if a new window is created.

```yaml
Type: System.UInt32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -XNumCharacters
Screen buffer width, in character columns, if a new console window is created.
This property is ignored in a GUI process.

```yaml
Type: System.UInt32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -XSize
Width, in pixels, of a new window, if a new window is created.

```yaml
Type: System.UInt32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -YCoordinate
Y-offset, in pixels, from the top edge of the screen to the top edge of the window, if a new window is created.

```yaml
Type: System.UInt32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -YNumCharacters
Screen buffer height, in character rows, if a new console window is created.
This property is ignored in a GUI process.

```yaml
Type: System.UInt32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -YSize
Height, in pixels, of the new window, if a new window is created.

```yaml
Type: System.UInt32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScriptingEngine
Name of the scripting engine to use, for example, "VBScript".
This property cannot be NULL.

```yaml
Type: System.String
Parameter Sets: ActiveScriptTextComputerSet, ActiveScriptFileComputerSet, ActiveScriptTextSessionSet, ActiveScriptFileSessionSet
Aliases:

Required: True
Position: Named
Default value: VBScript
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScriptText
Text of the script that is expressed in a language known to the scripting engine.
This property must be NULL if the ScriptFileName property is not NULL.

```yaml
Type: System.String
Parameter Sets: ActiveScriptTextComputerSet, ActiveScriptTextSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScriptFileName
Name of the file from which the script text is read, intended as an alternative to specifying the text of the script in the ScriptText property.
This property must be NULL if the ScriptText property is not NULL.

```yaml
Type: System.String
Parameter Sets: ActiveScriptFileComputerSet, ActiveScriptFileSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CimSession


```yaml
Type: Microsoft.Management.Infrastructure.CimSession[]
Parameter Sets: SMTPSessionSet, NtEventLogSessionSet, LogFileSessionSet, CommandLineTemplateSessionSet, CommandLineSessionSet, ActiveScriptTextSessionSet, ActiveScriptFileSessionSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential


```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: SMTPComputerSet, NtEventLogComputerSet, LogFileComputerSet, CommandLineTemplateComputerSet, CommandLineComputerSet, ActiveScriptTextComputerSet, ActiveScriptFileComputerSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ThrottleLimit


```yaml
Type: System.Int32
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

### System.String[]
## OUTPUTS

## NOTES

## RELATED LINKS
