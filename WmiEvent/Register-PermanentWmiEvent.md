---
external help file: WmiEvent-help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# Register-PermanentWmiEvent

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### SMTPComputerSet
```
Register-PermanentWmiEvent [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 -EventNamespace <String> -Query <String> -QueryLanguage <String> [<CommonParameters>]
```

### NtEventLogComputerSet
```
Register-PermanentWmiEvent [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 -EventNamespace <String> -Query <String> -QueryLanguage <String> [-Category <UInt16>] -EventID <UInt32>
 [-EventType <UInt32>] [-InsertionStringTemplates <String[]>] -NameOfUserSidProperty <String>
 -NameOfRawDataProperty <String> -SourceName <String> [-UNCServerName <String>] [<CommonParameters>]
```

### LogFileComputerSet
```
Register-PermanentWmiEvent [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 -EventNamespace <String> -Query <String> -QueryLanguage <String> -Filename <String> [-IsUnicode <Boolean>]
 [-MaximumFileSize <UInt64>] -Text <String> [<CommonParameters>]
```

### CommandLineTemplateComputerSet
```
Register-PermanentWmiEvent [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 -EventNamespace <String> -Query <String> -QueryLanguage <String> [-KillTimeout <UInt32>]
 -CommandLineTemplate <String> [-CreateNewProcessGroup <Boolean>] [-CreateSeparateWowVdm <Boolean>]
 [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>] [-ForceOnFeedback <Boolean>] [-Priority <Int32>]
 [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>] [-UseDefaultErrorMode <Boolean>]
 [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>] [-XNumCharacters <UInt32>]
 [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>] [-YSize <UInt32>] [<CommonParameters>]
```

### CommandLineComputerSet
```
Register-PermanentWmiEvent [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 -EventNamespace <String> -Query <String> -QueryLanguage <String> [-KillTimeout <UInt32>]
 -ExecutablePath <String> [-CreateNewProcessGroup <Boolean>] [-CreateSeparateWowVdm <Boolean>]
 [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>] [-ForceOnFeedback <Boolean>] [-Priority <Int32>]
 [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>] [-UseDefaultErrorMode <Boolean>]
 [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>] [-XNumCharacters <UInt32>]
 [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>] [-YSize <UInt32>] [<CommonParameters>]
```

### ActiveScriptTextComputerSet
```
Register-PermanentWmiEvent [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 -EventNamespace <String> -Query <String> -QueryLanguage <String> [-KillTimeout <UInt32>]
 -ScriptingEngine <String> -ScriptText <String> [<CommonParameters>]
```

### ActiveScriptFileComputerSet
```
Register-PermanentWmiEvent [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 -EventNamespace <String> -Query <String> -QueryLanguage <String> [-KillTimeout <UInt32>]
 -ScriptingEngine <String> -ScriptFileName <String> [<CommonParameters>]
```

### SMTPSessionSet
```
Register-PermanentWmiEvent -CimSession <CimSession[]> -Name <String> -EventNamespace <String> -Query <String>
 -QueryLanguage <String> [<CommonParameters>]
```

### NtEventLogSessionSet
```
Register-PermanentWmiEvent -CimSession <CimSession[]> -Name <String> -EventNamespace <String> -Query <String>
 -QueryLanguage <String> [-Category <UInt16>] -EventID <UInt32> [-EventType <UInt32>]
 [-InsertionStringTemplates <String[]>] -NameOfUserSidProperty <String> -NameOfRawDataProperty <String>
 -SourceName <String> [-UNCServerName <String>] [<CommonParameters>]
```

### LogFileSessionSet
```
Register-PermanentWmiEvent -CimSession <CimSession[]> -Name <String> -EventNamespace <String> -Query <String>
 -QueryLanguage <String> -Filename <String> [-IsUnicode <Boolean>] [-MaximumFileSize <UInt64>] -Text <String>
 [<CommonParameters>]
```

### CommandLineTemplateSessionSet
```
Register-PermanentWmiEvent -CimSession <CimSession[]> -Name <String> -EventNamespace <String> -Query <String>
 -QueryLanguage <String> [-KillTimeout <UInt32>] -CommandLineTemplate <String>
 [-CreateNewProcessGroup <Boolean>] [-CreateSeparateWowVdm <Boolean>] [-CreateSharedWowVdm <Boolean>]
 [-ForceOffFeedback <Boolean>] [-ForceOnFeedback <Boolean>] [-Priority <Int32>] [-RunInteractively <Boolean>]
 [-ShowWindowCommand <UInt32>] [-UseDefaultErrorMode <Boolean>] [-WindowTitle <String>]
 [-WorkingDirectory <String>] [-XCoordinate <UInt32>] [-XNumCharacters <UInt32>] [-XSize <UInt32>]
 [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>] [-YSize <UInt32>] [<CommonParameters>]
```

### CommandLineSessionSet
```
Register-PermanentWmiEvent -CimSession <CimSession[]> -Name <String> -EventNamespace <String> -Query <String>
 -QueryLanguage <String> [-KillTimeout <UInt32>] -ExecutablePath <String> [-CreateNewProcessGroup <Boolean>]
 [-CreateSeparateWowVdm <Boolean>] [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>]
 [-ForceOnFeedback <Boolean>] [-Priority <Int32>] [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>]
 [-UseDefaultErrorMode <Boolean>] [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>]
 [-XNumCharacters <UInt32>] [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>]
 [-YSize <UInt32>] [<CommonParameters>]
```

### ActiveScriptTextSessionSet
```
Register-PermanentWmiEvent -CimSession <CimSession[]> -Name <String> -EventNamespace <String> -Query <String>
 -QueryLanguage <String> [-KillTimeout <UInt32>] -ScriptingEngine <String> -ScriptText <String>
 [<CommonParameters>]
```

### ActiveScriptFileSessionSet
```
Register-PermanentWmiEvent -CimSession <CimSession[]> -Name <String> -EventNamespace <String> -Query <String>
 -QueryLanguage <String> [-KillTimeout <UInt32>] -ScriptingEngine <String> -ScriptFileName <String>
 [<CommonParameters>]
```

### SmtpSessionSet
```
Register-PermanentWmiEvent -Name <String> -EventNamespace <String> -Query <String> -QueryLanguage <String>
 [-BccLine <String>] [-CcLine <String>] [-FromLine <String>] [-HeaderFields <String[]>] -Message <String>
 [-ReplyToLine <String>] -SMTPServer <String> [-Subject <String>] -ToLine <String> [<CommonParameters>]
```

### SmtpComputerSet
```
Register-PermanentWmiEvent -Name <String> -EventNamespace <String> -Query <String> -QueryLanguage <String>
 [-BccLine <String>] [-CcLine <String>] [-FromLine <String>] [-HeaderFields <String[]>] -Message <String>
 [-ReplyToLine <String>] -SMTPServer <String> [-Subject <String>] -ToLine <String> [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -BccLine
{{ Fill BccLine Description }}

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

### -Category
{{ Fill Category Description }}

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

### -CcLine
{{ Fill CcLine Description }}

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

### -CimSession
{{ Fill CimSession Description }}

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

### -CommandLineTemplate
{{ Fill CommandLineTemplate Description }}

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

### -ComputerName
{{ Fill ComputerName Description }}

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

### -CreateNewProcessGroup
{{ Fill CreateNewProcessGroup Description }}

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
{{ Fill CreateSeparateWowVdm Description }}

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
{{ Fill CreateSharedWowVdm Description }}

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

### -Credential
{{ Fill Credential Description }}

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

### -EventID
{{ Fill EventID Description }}

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

### -EventNamespace
{{ Fill EventNamespace Description }}

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

### -EventType
{{ Fill EventType Description }}

```yaml
Type: System.UInt32
Parameter Sets: NtEventLogComputerSet, NtEventLogSessionSet
Aliases:
Accepted values: 0, 1, 2, 4, 8, 16

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExecutablePath
{{ Fill ExecutablePath Description }}

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

### -Filename
{{ Fill Filename Description }}

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

### -ForceOffFeedback
{{ Fill ForceOffFeedback Description }}

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
{{ Fill ForceOnFeedback Description }}

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

### -FromLine
{{ Fill FromLine Description }}

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
{{ Fill HeaderFields Description }}

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

### -InsertionStringTemplates
{{ Fill InsertionStringTemplates Description }}

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

### -IsUnicode
{{ Fill IsUnicode Description }}

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

### -KillTimeout
{{ Fill KillTimeout Description }}

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

### -MaximumFileSize
{{ Fill MaximumFileSize Description }}

```yaml
Type: System.UInt64
Parameter Sets: LogFileComputerSet, LogFileSessionSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Message
{{ Fill Message Description }}

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

### -Name
{{ Fill Name Description }}

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

### -NameOfRawDataProperty
{{ Fill NameOfRawDataProperty Description }}

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

### -NameOfUserSidProperty
{{ Fill NameOfUserSidProperty Description }}

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

### -Priority
{{ Fill Priority Description }}

```yaml
Type: System.Int32
Parameter Sets: CommandLineTemplateComputerSet, CommandLineComputerSet, CommandLineTemplateSessionSet, CommandLineSessionSet
Aliases:
Accepted values: 32, 64, 128, 256

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Query
{{ Fill Query Description }}

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

### -QueryLanguage
{{ Fill QueryLanguage Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: WQL

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplyToLine
{{ Fill ReplyToLine Description }}

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

### -RunInteractively
{{ Fill RunInteractively Description }}

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

### -SMTPServer
{{ Fill SMTPServer Description }}

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

### -ScriptFileName
{{ Fill ScriptFileName Description }}

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

### -ScriptText
{{ Fill ScriptText Description }}

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

### -ScriptingEngine
{{ Fill ScriptingEngine Description }}

```yaml
Type: System.String
Parameter Sets: ActiveScriptTextComputerSet, ActiveScriptFileComputerSet, ActiveScriptTextSessionSet, ActiveScriptFileSessionSet
Aliases:
Accepted values: VBScript, jscript

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShowWindowCommand
{{ Fill ShowWindowCommand Description }}

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

### -SourceName
{{ Fill SourceName Description }}

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

### -Subject
{{ Fill Subject Description }}

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

### -Text
{{ Fill Text Description }}

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

### -ToLine
{{ Fill ToLine Description }}

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

### -UNCServerName
{{ Fill UNCServerName Description }}

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

### -UseDefaultErrorMode
{{ Fill UseDefaultErrorMode Description }}

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
{{ Fill WindowTitle Description }}

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
{{ Fill WorkingDirectory Description }}

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
{{ Fill XCoordinate Description }}

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
{{ Fill XNumCharacters Description }}

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
{{ Fill XSize Description }}

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
{{ Fill YCoordinate Description }}

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
{{ Fill YNumCharacters Description }}

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
{{ Fill YSize Description }}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
