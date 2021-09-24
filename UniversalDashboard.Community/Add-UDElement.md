---
external help file: UniversalDashboard.Community-help.xml
Module Name: UniversalDashboard.Community
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDTreeView.md
schema: 2.0.0
---

# Add-UDElement

## SYNOPSIS
Adds a new element to the specified parent.

## SYNTAX

```
Add-UDElement -ParentId <String> [-Content <ScriptBlock>] [-Broadcast] [<CommonParameters>]
```

## DESCRIPTION
Adds a new element to the specified parent.
This will add the element after existing children.

## EXAMPLES

### Example 1
```
PS C:\> Set-UDElement -Id "message" -Attributes @{ 
                                type = "text"
                                value = ''
                                placeholder = "Type a chat message" 
                            }

PS C:\> Add-UDElement -ParentId "chatroom" -Content { $message } -Broadcast
```

Adds a message element the "chatroom" parent element.
It will add this element to all connected clients.

## PARAMETERS

### -Broadcast
Add the element to all connected clients.
If you don't specify this Switch, the element will only be added to whoever is interacting with the website.

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

### -Content
The content to append to the parent element.

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ParentId
The ID of the parent element.

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

### None
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
