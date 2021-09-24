---
external help file: WmiEvent-Help.xml
Module Name: WmiEvent
online version:
schema: 2.0.0
---

# New-CommandLineEventConsumer

## SYNOPSIS

## SYNTAX

### ExecutablePathByComputerName
```
New-CommandLineEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] -ExecutablePath <String> [-CreateNewProcessGroup <Boolean>]
 [-CreateSeparateWowVdm <Boolean>] [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>]
 [-ForceOnFeedback <Boolean>] [-Priority <Int32>] [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>]
 [-UseDefaultErrorMode <Boolean>] [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>]
 [-XNumCharacters <UInt32>] [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>]
 [-YSize <UInt32>] [<CommonParameters>]
```

### CommandLineTemplateByComputerName
```
New-CommandLineEventConsumer [-ComputerName <String[]>] [-Credential <PSCredential>] -Name <String>
 [-ThrottleLimit <Int32>] -CommandLineTemplate <String> [-CreateNewProcessGroup <Boolean>]
 [-CreateSeparateWowVdm <Boolean>] [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>]
 [-ForceOnFeedback <Boolean>] [-Priority <Int32>] [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>]
 [-UseDefaultErrorMode <Boolean>] [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>]
 [-XNumCharacters <UInt32>] [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>]
 [-YSize <UInt32>] [<CommonParameters>]
```

### ExecutablePathBySession
```
New-CommandLineEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>]
 -ExecutablePath <String> [-CreateNewProcessGroup <Boolean>] [-CreateSeparateWowVdm <Boolean>]
 [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>] [-ForceOnFeedback <Boolean>] [-Priority <Int32>]
 [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>] [-UseDefaultErrorMode <Boolean>]
 [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>] [-XNumCharacters <UInt32>]
 [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>] [-YSize <UInt32>] [<CommonParameters>]
```

### CommandLineTemplateBySession
```
New-CommandLineEventConsumer -CimSession <CimSession[]> -Name <String> [-ThrottleLimit <Int32>]
 -CommandLineTemplate <String> [-CreateNewProcessGroup <Boolean>] [-CreateSeparateWowVdm <Boolean>]
 [-CreateSharedWowVdm <Boolean>] [-ForceOffFeedback <Boolean>] [-ForceOnFeedback <Boolean>] [-Priority <Int32>]
 [-RunInteractively <Boolean>] [-ShowWindowCommand <UInt32>] [-UseDefaultErrorMode <Boolean>]
 [-WindowTitle <String>] [-WorkingDirectory <String>] [-XCoordinate <UInt32>] [-XNumCharacters <UInt32>]
 [-XSize <UInt32>] [-YCoordinate <UInt32>] [-YNumCharacters <UInt32>] [-YSize <UInt32>] [<CommonParameters>]
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
Parameter Sets: ExecutablePathBySession, CommandLineTemplateBySession
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
Parameter Sets: CommandLineTemplateByComputerName, CommandLineTemplateBySession
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
Parameter Sets: ExecutablePathByComputerName, CommandLineTemplateByComputerName
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: ExecutablePathByComputerName, CommandLineTemplateByComputerName
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExecutablePath


```yaml
Type: System.String
Parameter Sets: ExecutablePathByComputerName, ExecutablePathBySession
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
Parameter Sets: (All)
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

### -Priority


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

### -RunInteractively


```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShowWindowCommand


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

### -UseDefaultErrorMode


```yaml
Type: System.Boolean
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
