---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# New-UDSideNavItem

## SYNOPSIS
Creates a side navigation menu item.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-UDSideNavItem [-Background <String>] [-Children <ScriptBlock>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
New-UDSideNavItem [-Background <String>] [-Divider] [<CommonParameters>]
```

## DESCRIPTION
Creates a side navigation menu item.

## EXAMPLES

### Example 1
```
$Page1 = New-UDPage -Name "Page Name" -Content { New-UDCard -Id 'page-1' }
$Page2 = New-UDPage -Name "Page Name 2" -Content { New-UDCard -Id 'page-2'}

$Navigation = New-UDSideNav -Content {
    New-UDSideNavItem -Text "My First Page" -PageName "Page Name" -Icon group
    New-UDSideNavItem -Text "My Second Page" -PageName "Page Name 2" -Icon User
    New-UDSideNavItem -Text "Google" -Url 'https://www.google.com' -Icon Users
}

$Dashboard = New-UDDashboard -Title "Navigation" -Pages @($Page1, $Page2) -Navigation $Navigation
```

Creates a static navigation menu based on the SideNavItems listed in the content.

### Example 2
```
$Page1 = New-UDPage -Name "Page Name" -Content { New-UDCard -Id 'page-1' }
$Page2 = New-UDPage -Name "Page Name 2" -Content { New-UDCard -Id 'page-2'}

$Navigation = New-UDSideNav -None

New-UDDashboard -Title "Navigation" -Pages @($Page1, $Page2) -Navigation $Navigation
```

Hides the side navigation menu and hamburger icon.

### Example 3
```
$Page1 = New-UDPage -Name "Page Name" -Content { New-UDCard -Id 'page-1' }
$Page2 = New-UDPage -Name "Page Name 2" -Content { New-UDCard -Id 'page-2'}

$Navigation = New-UDSideNav -Content {
    New-UDSideNavItem -Text "Section" -Children {
        New-UDSideNavItem -Text "My Second Page" -PageName "Page Name 2" -Icon User
        New-UDSideNavItem -Text "Google" -Url 'https://www.google.com' -Icon Users
    }
} -Fixed

New-UDDashboard -Title "Navigation" -Pages @($Page1, $Page2) -Navigation $Navigation
```

Creates a side navigation menu with nested items with a fixed menu.

### Example 4
```
$Page1 = New-UDPage -Name "Page Name" -Content { New-UDCard -Id 'page-1' }
$Page2 = New-UDPage -Name "Page Name 2" -Content { New-UDCard -Id 'page-2'}

$Navigation = New-UDSideNav -Content {
    New-UDSideNavItem -Text "My First Page" -PageName "Page Name" -Icon group
    New-UDSideNavItem -Subheader -Text "Subheader"
    New-UDSideNavItem -Text "My Second Page" -PageName "Page Name 2" -Icon User
    New-UDSideNavItem -Divider
    New-UDSideNavItem -Text "Google" -Url 'https://www.google.com' -Icon Users
} -Fixed

New-UDDashboard -Title "Navigation" -Pages @($Page1, $Page2) -Navigation $Navigation
```

Creates a side menu with sub headers and a divider.

### Example 5
```
$Page1 = New-UDPage -Name "Page Name" -Content { New-UDCard -Id 'page-1' }
$Page2 = New-UDPage -Name "Page Name 2" -Content { New-UDCard -Id 'page-2'}

$Navigation = New-UDSideNav -Endpoint {
    New-UDSideNavItem -Text "My First Page" -OnClick { Show-UDModal -Content { New-UDCard -Id "ModalCard" } } -Icon group
} -Fixed

New-UDDashboard -Title "Navigation" -Pages @($Page1, $Page2) -Navigation $Navigation
```

Loads a side menu dynamically from an endpoint.

## PARAMETERS

### -Background
{{Fill Background Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Children
Adds children to this side navigation item.
This creates a drop down element.

```yaml
Type: ScriptBlock
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Divider
Inserts a divider into the side navigation menu.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
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

### None
## OUTPUTS

### System.Object
## NOTES
*

## RELATED LINKS
