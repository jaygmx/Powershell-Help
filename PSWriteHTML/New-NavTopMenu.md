---
external help file: PSWriteHTML-help.xml
Module Name: PSWriteHTML
online version:
schema: 2.0.0
---

# New-NavTopMenu

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### FontAwesomeSolid (Default)
```
New-NavTopMenu [[-MenuItem] <ScriptBlock>] -Name <String> [-Href <String>] [-InternalPageID <String>]
 [-IconColor <String>] [-IconSolid <String>] [<CommonParameters>]
```

### FontMaterial
```
New-NavTopMenu [[-MenuItem] <ScriptBlock>] -Name <String> [-Href <String>] [-InternalPageID <String>]
 [-IconColor <String>] [-IconMaterial <String>] [-Spinning] [-SpinningReverse] [-Bordered] [-BorderedCircle]
 [-PullLeft] [-PullRight] [-Rotate <String>] [-FlipVertical] [-FlipHorizontal] [<CommonParameters>]
```

### FontAwesomeRegular
```
New-NavTopMenu [[-MenuItem] <ScriptBlock>] -Name <String> [-Href <String>] [-InternalPageID <String>]
 [-IconColor <String>] [-IconRegular <String>] [<CommonParameters>]
```

### FontAwesomeBrands
```
New-NavTopMenu [[-MenuItem] <ScriptBlock>] -Name <String> [-Href <String>] [-InternalPageID <String>]
 [-IconColor <String>] [-IconBrands <String>] [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Bordered
{{ Fill Bordered Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontMaterial
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BorderedCircle
{{ Fill BorderedCircle Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontMaterial
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FlipHorizontal
{{ Fill FlipHorizontal Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontMaterial
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FlipVertical
{{ Fill FlipVertical Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontMaterial
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Href
{{ Fill Href Description }}

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

### -IconBrands
{{ Fill IconBrands Description }}

```yaml
Type: System.String
Parameter Sets: FontAwesomeBrands
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconColor
{{ Fill IconColor Description }}

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

### -IconMaterial
{{ Fill IconMaterial Description }}

```yaml
Type: System.String
Parameter Sets: FontMaterial
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconRegular
{{ Fill IconRegular Description }}

```yaml
Type: System.String
Parameter Sets: FontAwesomeRegular
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconSolid
{{ Fill IconSolid Description }}

```yaml
Type: System.String
Parameter Sets: FontAwesomeSolid
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InternalPageID
{{ Fill InternalPageID Description }}

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

### -MenuItem
{{ Fill MenuItem Description }}

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
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

### -PullLeft
{{ Fill PullLeft Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontMaterial
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PullRight
{{ Fill PullRight Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontMaterial
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Rotate
{{ Fill Rotate Description }}

```yaml
Type: System.String
Parameter Sets: FontMaterial
Aliases:
Accepted values: 90, 180, 270

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Spinning
{{ Fill Spinning Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontMaterial
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SpinningReverse
{{ Fill SpinningReverse Description }}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: FontMaterial
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

### None

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
