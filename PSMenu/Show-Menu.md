---
external help file: PSMenu-help.xml
Module Name: PSMenu
online version: https://github.com/Sebazzz/PSMenu
schema: 2.0.0
---

# Show-Menu

## SYNOPSIS
Shows an interactive menu to the user and returns the chosen item or item index.

## SYNTAX

```
Show-Menu [-MenuItems] <Array> [-ReturnIndex] [-MultiSelect] [-ItemFocusColor <ConsoleColor>]
 [-MenuItemFormatter <ScriptBlock>] [-InitialSelection <Array>] [<CommonParameters>]
```

## DESCRIPTION
Shows an interactive menu on supporting console hosts.
The user can interactively
select one (or more, in case of -MultiSelect) items.
The cmdlet returns the items
itself, or its indices (in case of -ReturnIndex). 

The interactive menu is controllable by hotkeys:
- Arrow up/down: Focus menu item.
- Enter: Select menu item.
- Page up/down: Go one page up or down - if the menu is larger then the screen.
- Home/end: Go to the top or bottom of the menu.
- Spacebar: If in multi-select mode (MultiSelect parameter), toggle item choice.

Not all console hosts support the interactive menu (PowerShell ISE is a well-known
host which doesn't support it).
The console host needs to support the ReadKey method.
The default PowerShell console host does this.

## EXAMPLES

### EXAMPLE 1
```
Show-Menu @("option 1", "option 2", "option 3")
```

### EXAMPLE 2
```
Show-Menu -MenuItems $(Get-NetAdapter) -MenuItemFormatter { $Args | Select -Exp Name }
```

### EXAMPLE 3
```
Show-Menu @("Option A", "Option B", $(Get-MenuSeparator), "Quit")
```

## PARAMETERS

### -MenuItems
Array of objects or strings containing menu items.
Must contain at least one item.
Must not contain $null. 

The items are converted to a string for display by the MenuItemFormatter parameter, which
does by default a ".ToString()" of the underlying object.
It is best for this string 
to fit on a single line.

The array of menu items may also contain unselectable separators, which can be used
to visually distinct menu items.
You can call Get-MenuSeparator to get a separator object,
and add that to the menu item array.

```yaml
Type: System.Array
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReturnIndex
Instead of returning the object(s) that has/have been chosen, return the index/indices
of the object(s) that have been chosen.

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

### -MultiSelect
Allow the user to select multiple items instead of a single item.

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

### -ItemFocusColor
The console color used for focusing the active item.
This by default green,
which looks good on both default PowerShell-blue and black consoles.

```yaml
Type: System.ConsoleColor
Parameter Sets: (All)
Aliases:
Accepted values: Black, DarkBlue, DarkGreen, DarkCyan, DarkRed, DarkMagenta, DarkYellow, Gray, DarkGray, Blue, Green, Cyan, Red, Magenta, Yellow, White

Required: False
Position: Named
Default value: Green
Accept pipeline input: False
Accept wildcard characters: False
```

### -MenuItemFormatter
A function/scriptblock which accepts a menu item (from the MenuItems parameter)
and returns a string suitable for display.
This function will be called many times,
for each menu item once.

This parameter is optional and by default executes a ".ToString()" on the object.
If you control the objects that you pass in MenuItems, then you want to probably
override the ToString() method.
If you don't control the objects, then this parameter
is very useful.

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: { Param($M) Format-MenuItemDefault $M }
Accept pipeline input: False
Accept wildcard characters: False
```

### -InitialSelection
Set initial selections if multi-select mode.
This is an array of indecies.

```yaml
Type: System.Array
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

### None. You cannot pipe objects to Show-Menu.
## OUTPUTS

### Array of chosen menu items or (if the -ReturnIndex parameter is given) the indices.
## NOTES

## RELATED LINKS

[https://github.com/Sebazzz/PSMenu](https://github.com/Sebazzz/PSMenu)

