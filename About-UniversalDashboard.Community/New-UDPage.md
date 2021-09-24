---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDMonitor.md
schema: 2.0.0
---

# New-UDPage

## SYNOPSIS
Creates a new page in the dashboard.

## SYNTAX

```
New-UDPage [[-Content] <ScriptBlock>] [-DefaultHomePage] [-ArgumentList <Object[]>] [-AutoRefresh]
 [-Endpoint <ScriptBlock>] [<CommonParameters>]
```

## DESCRIPTION
Creates a new page in the dashboard.

## EXAMPLES

### Example 1
```
PS C:\> $Page1 = New-UDPage -Name "Home" -Content { New-Chart... }
PS C:\> $Page2 = New-UDPage -Name "Cards" -Content { New-Card... }

PS C:\> $Dashboard = New-UDDashboard -Color "blue" -Pages @($Page1, $Page2)
```

Creates a multi-page dashboard.
The will show a navigation pane on the left side of the dashboard to navigate to different pages.

### Example 2
```
PS C:\> $Page1 = New-UDPage -Name "Home" -Content { New-Chart... }
PS C:\> $Page2 = New-UDPage -Name "Cards" -Url "/cards-page" -Content { New-Card... }

PS C:\> $Dashboard = New-UDDashboard -Color "blue" -Pages @($Page1, $Page2)
```

Creates a multi-page dashboard.
The will show a navigation pane on the left side of the dashboard to navigate to different pages.
The URL for the cards page is /cards-page.

### Example 3
```
PS C:\> $Page1 = New-UDPage -Name "Home" -Content { New-Chart... }
PS C:\> $Page2 = New-UDPage -Name "Cards" -Url "/cards-page/:username" -Content { New-Card -Title $username }

PS C:\> $Dashboard = New-UDDashboard -Color "blue" -Pages @($Page1, $Page2)
```

Creates a multi-page dashboard.
The will show a navigation pane on the left side of the dashboard to navigate to different pages.
The URL for the cards page is /cards-page/:username.
The :username portion of the URL can be replaced with any string.
The variable $username will be available in the endpoint that generates the page.

### Example 4
```
PS C:\> $Page1 = New-UDPage -Name "Home" -Content { New-Chart... }
PS C:\> $Page2 = New-UDPage -Name "Demo" -DefaultHomePage -Content { New-Chart... }

PS C:\> $Dashboard = New-UDDashboard -Color "blue" -Pages @($Page1, $Page2)
```

Creates a multi-page dashboard.
The will show a navigation pane on the left side of the dashboard to navigate to different pages.
The default home page will be Demo and NOT home.
The dashboard title will also be linked to the default home page.

## PARAMETERS

### -ArgumentList
Arguments to pass to the endpoint.
They will be available via the $ArgumentList variable.

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutoRefresh
Auth refresh this page.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Content
The content of the page.
This can be any set of controls you would pass to the Content parameter of New-UDDashboard.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultHomePage
Set the default home page for the dashboard and Set the dashboard title bar as link to the home page.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Endpoint
Endpoint that is called to generate the content for this page.

```yaml
Type: ScriptBlock
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
