---
external help file: WmiEvent-help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# Register-PermanentWmiEvent

## SYNOPSIS


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

```



## PARAMETERS

### -BccLine


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
