---
external help file: WmiEvent-Help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# New-ActiveScriptEventConsumer

## SYNOPSIS

## SYNTAX

### ScriptTextByComputerName
```
New-ActiveScriptEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>] -ScriptingEngine <String> -ScriptText <String>
 [<CommonParameters>]
```

### FileNameByComputerName
```
New-ActiveScriptEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-KillTimeout <UInt32>] -ScriptingEngine <String> -ScriptFileName <String>
 [<CommonParameters>]
```

### ScriptTextBySession
```
New-ActiveScriptEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>]
 [-KillTimeout <UInt32>] -ScriptingEngine <String> -ScriptText <String> [<CommonParameters>]
```

### FileNameBySession
```
New-ActiveScriptEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>]
 [-KillTimeout <UInt32>] -ScriptingEngine <String> -ScriptFileName <String> [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -CimSession


```yaml
Type: Microsoft.Management.Infrastructure.CimSession[]
Parameter Sets: ScriptTextBySession, FileNameBySession
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
Parameter Sets: ScriptTextByComputerName, FileNameByComputerName
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
Parameter Sets: ScriptTextByComputerName, FileNameByComputerName
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
Parameter Sets: (All)
Aliases:

Required: False
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

### -ScriptFileName


```yaml
Type: System.String
Parameter Sets: FileNameByComputerName, FileNameBySession
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
Parameter Sets: (All)
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
Parameter Sets: ScriptTextByComputerName, ScriptTextBySession
Aliases:

Required: True
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

## OUTPUTS

## NOTES

## RELATED LINKS
