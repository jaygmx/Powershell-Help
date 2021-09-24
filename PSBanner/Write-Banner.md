---
external help file: PSBanner-help.xml
Module Name: PSBanner
online version:
schema: 2.0.0
---

# Write-Banner

## SYNOPSIS
Write banner string to the console.

## SYNTAX

```
Write-Banner [-InputObject] <PSObject> [-FontName <String>] [-FontSize <Int32>] [-Bold] [-Italic] [-Strikeout]
 [-Underline] [-Stream] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```



## PARAMETERS

### -InputObject
Specify the object to write banner string.
if the object's type is not string, "Name" property value or "ToString()" method result is choosen.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -FontName
Specify the font family name.
Get-FontFamilies cmdlet can get all available font family names.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: f

Required: False
Position: Named
Default value: Consolas
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontSize
Font size(pt).

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases: s

Required: False
Position: Named
Default value: 10
Accept pipeline input: False
Accept wildcard characters: False
```

### -Bold
Specify using Bold for font style.

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

### -Italic
Specify using Italic for font style.

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

### -Strikeout
Specify using Strikeout for font style.

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

### -Underline
Specify using Underline for font style.

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

### -Stream
Default false.

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

## RELATED LINKS
