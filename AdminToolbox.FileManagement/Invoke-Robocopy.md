---
external help file: AdminToolbox.FileManagement-help.xml
Module Name: AdminToolbox.FileManagement
online version:
schema: 2.0.0
---

# Invoke-Robocopy

## SYNOPSIS

## SYNTAX

### NoPurgeSync
```
Invoke-Robocopy [-Source] <Object> [-Target] <Object> [-Arguments <Object>] [-NoPurgeSync] [<CommonParameters>]
```

### NoPreset
```
Invoke-Robocopy [-Source] <Object> [-Target] <Object> [-Nopreset] [-Arguments <Object>] [<CommonParameters>]
```

### MirrorSync
```
Invoke-Robocopy [-Source] <Object> [-Target] <Object> [-Arguments <Object>] [-MirrorSync] [<CommonParameters>]
```

## DESCRIPTION
This is a wrapper function that provides preset robocopy options using parameter sets and supports running with no presets.

## EXAMPLES

### EXAMPLE 1
```
The NoPresets parameter set allows for specifying all arguments in any combination that is preferred.
```

$Arguments = @("/mir", "/copyall", "/r:1", "/w:1", "/zb", "/E")
$Arguments | Invoke-Robocopy -Source c:\temp -Target c:\test -nopreset

or

Invoke-Robocopy -Nopreset -Source c:\temp -Target c:\test -Arguments "/mir", "/copyall", "/r:1", "/w:1", "/zb", "

### EXAMPLE 2
```
Default set of parameters for mirroring directories with permissions and purging files that no longer exist at the source.
#Command run is equal to <Robocopy.exe $Source $Target /mir /COPY:DATSO /r:1 /w:1 /zb $Arguments>
```

Invoke-Robocopy -Source c:\temp -Target c:\test -MirrorSync

### EXAMPLE 3
```
Default set of parameters for mirroring directories with permissions without purging files that no longer exist at the source.
#Command run is equal to <Robocopy.exe $Source $Target /e /COPY:DATSO /r:1 /w:1 /zb $Arguments>
```

Invoke-Robocopy -Source c:\temp -Target c:\test -NoPurgeSync

## PARAMETERS

### -Source
Source directory from which files are being copied from

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Target
The target directory for copied files

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Nopreset
Specifies that you will be providing your own parameter set for the Robocopy Job

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: NoPreset
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Arguments
Any combination of robocopy parameters that can be passed to the NoPreset paremeterset, or any prepopulated parametersets

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MirrorSync
Specifies that you wish to use the MirrorSync preset options for the Robocopy job

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: MirrorSync
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoPurgeSync
Specifies that you wish to use the NoPurgeSync preset options for the Robocopy job

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: NoPurgeSync
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
