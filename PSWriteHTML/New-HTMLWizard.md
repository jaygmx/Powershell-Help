---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-HTMLWizard

## SYNOPSIS
Provides a simple way to build wizard

## SYNTAX

```
New-HTMLWizard [[-WizardSteps] <ScriptBlock>] [[-Theme] <String>] [-DisableCycleSteps]
 [[-ToolbarPosition] <String>] [[-ToolbarButtonPosition] <String>] [-HideNextButton] [-HidePreviousButton]
 [-DiableAnchorClickable] [-EnableAllAnchors] [-DisableMarkDoneStep] [-DisableMarkAllPreviousStepsAsDone]
 [-RemoveDoneStepOnNavigateBack] [-DisableAnchorOnDoneStep] [-DisableJustification] [-DisableBackButtonSupport]
 [-DisableURLhash] [[-TransitionAnimation] <String>] [[-TransitionSpeed] <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Provides a simple way to build wizard

## EXAMPLES

### EXAMPLE 1
```
An example
```

## PARAMETERS

### -WizardSteps
{{ Fill WizardSteps Description }}

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

### -Theme
Choose a theme to display wizard in

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

### -DisableCycleSteps
Disables the navigation cycle through

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

### -ToolbarPosition
Position of the toolbar (none, top, bottom, both)

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

### -ToolbarButtonPosition
Button alignment of the toolbar (left, right, center)

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HideNextButton
Hide next button

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

### -HidePreviousButton
Hide previous button

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

### -DiableAnchorClickable
Disable anchor navigation

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

### -EnableAllAnchors
Activates all anchors clickable all times

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

### -DisableMarkDoneStep
Disable done state on navigation

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

### -DisableMarkAllPreviousStepsAsDone
Disable when a step selected by url hash, all previous steps are marked done

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

### -RemoveDoneStepOnNavigateBack
While navigate back done step after active step will be cleared

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

### -DisableAnchorOnDoneStep
Disable the done steps navigation

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
Position: 5
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
Position: 6
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Implementation based on: http://techlaboratory.net/jquery-smartwizard
License: MIT

## RELATED LINKS
