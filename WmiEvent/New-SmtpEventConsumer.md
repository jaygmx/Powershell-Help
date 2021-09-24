---
external help file: WmiEvent-Help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# New-SmtpEventConsumer

## SYNOPSIS

## SYNTAX

### ByComputerName
```
New-SmtpEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] [-BccLine <String>] [-CcLine <String>] [-FromLine <String>]
 [-HeaderFields <String[]>] -Message <String> [-ReplyToLine <String>] -SMTPServer <String> [-Subject <String>]
 -ToLine <String> [<CommonParameters>]
```

### BySession
```
New-SmtpEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>] [-BccLine <String>]
 [-CcLine <String>] [-FromLine <String>] [-HeaderFields <String[]>] -Message <String> [-ReplyToLine <String>]
 -SMTPServer <String> [-Subject <String>] -ToLine <String> [<CommonParameters>]
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
Parameter Sets: (All)
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

### -FromLine


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

### -HeaderFields


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

### -Message


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

### -ReplyToLine


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

### -SMTPServer


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

### -Subject


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

### -ToLine


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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
