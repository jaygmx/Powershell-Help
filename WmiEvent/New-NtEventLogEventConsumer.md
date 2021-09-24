---
external help file: WmiEvent-Help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# New-NtEventLogEventConsumer

## SYNOPSIS

## SYNTAX

### ByComputerName
```
New-NtEventLogEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-Category <UInt16>] -EventID <UInt32> [-EventType <UInt32>]
 [-InsertionStringTemplates <String[]>] -NameOfUserSidProperty <String> -NameOfRawDataProperty <String>
 -SourceName <String> [-UNCServerName <String>] [<CommonParameters>]
```

### BySession
```
New-NtEventLogEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>]
 [-Category <UInt16>] -EventID <UInt32> [-EventType <UInt32>] [-InsertionStringTemplates <String[]>]
 -NameOfUserSidProperty <String> -NameOfRawDataProperty <String> -SourceName <String> [-UNCServerName <String>]
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -Category


```yaml
Type: System.UInt16
Parameter Sets: (All)
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
Parameter Sets: BySession
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
Parameter Sets: ByComputerName
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
Parameter Sets: ByComputerName
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
Parameter Sets: (All)
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

### -NameOfRawDataProperty


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

### -NameOfUserSidProperty


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

### -SourceName


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

### -UNCServerName


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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
