---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# New-UDTreeNode

## SYNOPSIS
A node within a TreeView.

## SYNTAX

```
New-UDTreeNode [-Children <ScriptBlock>] [<CommonParameters>]
```

## DESCRIPTION
A node within a TreeView.

## EXAMPLES

### Example 1
```
PS C:\> New-UDTreeView -Node {
    New-UDTreeNode -Name "Root Node" -Children {
        New-UDTreeNode -Name "Child 1"
        New-UDTreeNode -Name "Child 2"
        New-UDTreeNode -Name "Child 3"
    }
}
```

Creates a tree view with 3 children nodes.

## PARAMETERS

### -Children
A script block that returns children nodes.

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
