---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLTabPanel

## SYNOPSIS
Flexible and easy to implement Tab Panel with a lot of features, cool animation effects, event support, easy to customize.

## SYNTAX

```
New-HTMLTabPanel [[-Tabs] <ScriptBlock>] [[-Orientation] <String>] [-DisableJustification]
 [-DisableBackButtonSupport] [-DisableURLhash] [[-TransitionAnimation] <String>] [[-TransitionSpeed] <Int32>]
 [-AutoProgress] [[-AutoProgressInterval] <Int32>] [-DisableAutoProgressStopOnFocus] [<CommonParameters>]
```

## DESCRIPTION
Flexible and easy to implement Tab Panel with a lot of features, cool animation effects, event support, easy to customize.

## EXAMPLES

### EXAMPLE 1
```
An example
```

## PARAMETERS

### -Tabs
{{ Fill Tabs Description }}

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Orientation
Nav menu orientation.
Default value is 'horizontal'.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisableJustification
Disable navigation menu justification

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisableBackButtonSupport
Disable the back button support

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisableURLhash
Disable selection of the tab based on url hash

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -TransitionAnimation
Effect on navigation, none/fade/slide-horizontal/slide-vertical/slide-swing

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TransitionSpeed
Transion animation speed.
Default 400

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutoProgress
Enables auto navigation

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutoProgressInterval
Auto navigate Interval (used only if "autoProgress" is enabled).
Default 3500

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisableAutoProgressStopOnFocus
Disable stop auto navigation on focus and resume on outfocus (used only if "autoProgress" is enabled)

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
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
Implementation based on: http://techlaboratory.net/jquery-smarttab
License: MIT

## RELATED LINKS
