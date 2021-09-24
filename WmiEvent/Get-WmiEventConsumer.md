---
external help file: WmiEvent-Help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# Get-WmiEventConsumer

## SYNOPSIS

## SYNTAX

### ByComputerName
```
Get-WmiEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] [-ThrottleLimit <Int32>]
 [<CommonParameters>]
```

### ByCimSession
```
Get-WmiEventConsumer -CimSession <CimSession[]> [-ThrottleLimit <Int32>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```
Get-WmiEventConsumer


ComputerName    : WIN-OL5AKAF1OUJ
Name            : AS_GenericHTTPPOST
ScriptingEngine : VBScript
ScriptFileName  :
ScriptText      : Set objHTTP = CreateObject("Microsoft.XMLHTTP")
                  objHTTP.open "POST", "http://10.20.3.139/", False

                  objHTTP.setRequestHeader "User-Agent", "DoYouEven-TF12-Bro?"

                  Dim outputString

                  outputString = outputString & "{'TargetEvent': {" & vbCrLf
                  outputString = outputString & vbTab & "'EventType': '" & TargetEvent.Path_.Class & "'," & vbCrLf
                  outputString = outputString & vbTab & "'TimeCreated': '" & TargetEvent.Time_Created & "'," & vbCrLf
                  outputString = outputString & vbTab & "'Server': '" & TargetEvent.Path_.Server & "'," & vbCrLf
                  outputString = outputString & vbTab & "'InstanceType': '" & TargetEvent.TargetInstance.Path_.Class &
                  "'," & vbCrLf
                  outputString = outputString & vbTab & "'TargetInstance': {" & vbCrLf

                  For Each oProp in TargetEvent.TargetInstance.Properties_
                       outputString = outputString & vbTab & vbTab & "'" & oProp.Name & "': '" & oProp & "'," & vbCrLf
                  Next

                  outputString = outputString & vbTab & "}" & vbCrLf
                  outputString = outputString & "}}"

                  objHTTP.send outputString

                  Set objHTTP = Nothing

ComputerName    : WIN-OL5AKAF1OUJ
Name            : AS_ExtrinsicHTTPPOST
ScriptingEngine : VBScript
ScriptFileName  :
ScriptText      : Set objSysInfo = CreateObject("WinNTSystemInfo")
                  Set objHTTP = CreateObject("Microsoft.XMLHTTP")

                  objHTTP.open "POST", "http://127.0.0.1/", False

                  objHTTP.setRequestHeader "User-Agent", "DoYouEven-TF12-Bro?"

                  Dim outputString

                  outputString = outputString & "{""TargetEvent"":{"
                  outputString = outputString & """EventType"":""ExtrinsicEvent"","
                  outputString = outputString & """TimeCreated"":""" & TargetEvent.Time_Created & ""","
                  outputString = outputString & """Server"":""" & objSysInfo.ComputerName & ""","
                  outputString = outputString & """InstanceType"":""" & TargetEvent.Path_.Class & ""","
                  outputString = outputString & """TargetInstance"":{"

                  For Each oProp in TargetEvent.Properties_
                       If oProp.Name <> "Sid" Then
                          outputString = outputString & """" & oProp.Name & """:" & """" & oProp & ""","
                      End If
                  Next

                  outputString = Left(outputString, Len(outputString) - 1)
                  outputString = outputString & "}"
                  outputString = outputString & "}}"

                  objHTTP.send outputString

                  Set objHTTP = Nothing
```

Gets all Event Consumers on localhost

### EXAMPLE 2
```
Get-WmiEventConsumer -ComputerName SERVER1


ComputerName    : SERVER1
Name            : AS_Test
ScriptingEngine : VBScript
ScriptFileName  :
ScriptText      : Set objHTTP = CreateObject("Microsoft.XMLHTTP")
                  objHTTP.open "POST", "http://127.0.0.1/", False

                  objHTTP.setRequestHeader "User-Agent", "DoYouEven-TF12-Bro?"

                  Dim outputString

                  outputString = outputString & "{""TargetEvent"":{"
                  outputString = outputString & """EventType"":""" & TargetEvent.Path_.Class & ""","
                  outputString = outputString & """TimeCreated"":""" & TargetEvent.Time_Created & ""","
                  outputString = outputString & """Server"":""" & TargetEvent.Path_.Server & ""","
                  outputString = outputString & """InstanceType"":""" & TargetEvent.TargetInstance.Path_.Class & ""","
                  outputString = outputString & """TargetInstance"": {"

                  For Each oProp in TargetEvent.TargetInstance.Properties_
                       outputString = outputString & """" & oProp.Name & """:""" & oProp & ""","
                  Next

                  outputString = Left(outputString, Len(outputString) - 3)
                  outputString = outputString & "}"
                  outputString = outputString & "}}"

                  outputString = Replace(outputString, "\", "\\")

                  objHTTP.send outputString

                  Set objHTTP = Nothing

ComputerName    : SERVER1
Name            : AS_ExtrinsicHTTPPOST
ScriptingEngine : VBScript
ScriptFileName  :
ScriptText      : Set objSysInfo = CreateObject("WinNTSystemInfo")
                  Set objHTTP = CreateObject("Microsoft.XMLHTTP")

                  objHTTP.open "POST", "http://127.0.0.1/", False

                  objHTTP.setRequestHeader "User-Agent", "DoYouEven-TF12-Bro?"

                  Dim outputString

                  outputString = outputString & "{""TargetEvent"":{"
                  outputString = outputString & """EventType"":""ExtrinsicEvent"","
                  outputString = outputString & """TimeCreated"":""" & TargetEvent.Time_Created & ""","
                  outputString = outputString & """Server"":""" & objSysInfo.ComputerName & ""","
                  outputString = outputString & """InstanceType"":""" & TargetEvent.Path_.Class & ""","
                  outputString = outputString & """TargetInstance"":{"

                  For Each oProp in TargetEvent.Properties_
                       If oProp.Name <> "Sid" Then
                          outputString = outputString & """" & oProp.Name & """:" & """" & oProp & ""","
                      End If
                  Next

                  outputString = Left(outputString, Len(outputString) - 1)
                  outputString = outputString & "}"
                  outputString = outputString & "}}"

                  objHTTP.send outputString

                  Set objHTTP = Nothing
```

Gets all Event Consumers on SERVER1

### EXAMPLE 3
```
Get-WmiEventConsumer -Name AS_Test


ComputerName    : WIN-OL5AKAF1OUJ
Name            : AS_Test
ScriptingEngine : VBScript
ScriptFileName  :
ScriptText      : Set objHTTP = CreateObject("Microsoft.XMLHTTP")
                  objHTTP.open "POST", "http://127.0.0.1/", False

                  objHTTP.setRequestHeader "User-Agent", "DoYouEven-TF12-Bro?"

                  Dim outputString

                  outputString = outputString & "{""TargetEvent"":{"
                  outputString = outputString & """EventType"":""" & TargetEvent.Path_.Class & ""","
                  outputString = outputString & """TimeCreated"":""" & TargetEvent.Time_Created & ""","
                  outputString = outputString & """Server"":""" & TargetEvent.Path_.Server & ""","
                  outputString = outputString & """InstanceType"":""" & TargetEvent.TargetInstance.Path_.Class & ""","
                  outputString = outputString & """TargetInstance"": {"

                  For Each oProp in TargetEvent.TargetInstance.Properties_
                       outputString = outputString & """" & oProp.Name & """:""" & oProp & ""","
                  Next

                  outputString = Left(outputString, Len(outputString) - 3)
                  outputString = outputString & "}"
                  outputString = outputString & "}}"

                  outputString = Replace(outputString, "\", "\\")

                  objHTTP.send outputString

                  Set objHTTP = Nothing
```

Returns the Event Consumer named AS_Test from the localhost

## PARAMETERS

### -ComputerName
Gets the Event Consumers running on the specified computers.
The default is the local computer.

Type the NetBIOS name, an IP address, or a fully qualified domain name of one or more computers.
To specify the local computer, type the computer name, a dot (.), or "localhost".

This parameter does not rely on Windows PowerShell remoting.
You can use the ComputerName parameter of Get-WmiEventConsumer even if your computer is not configured to run remote commands.

```yaml
Type: System.String[]
Parameter Sets: ByComputerName
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
Parameter Sets: ByCimSession
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
Parameter Sets: ByComputerName
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
