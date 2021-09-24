---
external help file: PSMenu-help.xml
Module Name: PSMenu
online version:
schema: 2.0.0
---

# Get-MenuSeparator

## SYNOPSIS
Returns a separator for the Show-Menu Cmdlet.
The separator is not selectable by the user and
allows a visual distinction of multiple menuitems.

## SYNTAX

```
Get-MenuSeparator [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### EXAMPLE 1
```
$MenuItems = @("Option A", "Option B", $(Get-MenuSeparator), "Quit")
Show-Menu $MenuItems
```

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
