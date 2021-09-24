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
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -CimSession
{{ Fill CimSession Description }}

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
{{ Fill CommandLineTemplate Description }}

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
{{ Fill ComputerName Description }}

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
{{ Fill CreateNewProcessGroup Description }}

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
{{ Fill CreateSeparateWowVdm Description }}

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
{{ Fill CreateSharedWowVdm Description }}

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
{{ Fill Credential Description }}

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
{{ Fill ExecutablePath Description }}

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
{{ Fill ForceOffFeedback Description }}

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
{{ Fill ForceOnFeedback Description }}

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

### -Priority
{{ Fill Priority Description }}

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
{{ Fill RunInteractively Description }}

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
{{ Fill ShowWindowCommand Description }}

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
{{ Fill ThrottleLimit Description }}

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
{{ Fill UseDefaultErrorMode Description }}

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
{{ Fill WindowTitle Description }}

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
{{ Fill WorkingDirectory Description }}

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
{{ Fill XCoordinate Description }}

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
{{ Fill XNumCharacters Description }}

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
{{ Fill XSize Description }}

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
{{ Fill YCoordinate Description }}

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
{{ Fill YNumCharacters Description }}

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
{{ Fill YSize Description }}

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
