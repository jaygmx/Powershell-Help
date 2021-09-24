---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Set-BitmapSize

## SYNOPSIS
PSCX Cmdlet: Sets the size of the specified bitmap.

## SYNTAX

### ExactSize
```
Set-BitmapSize [[-Width] <Int32>] [[-Height] <Int32>] [-KeepAspectRatio] [-Bitmap] <Bitmap>
 [<CommonParameters>]
```

### Percentage
```
Set-BitmapSize [-Percent] <Int32> [-Bitmap] <Bitmap> [<CommonParameters>]
```

## DESCRIPTION
Sets the size of the specified bitmap.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -Bitmap
The bitmap to process.

```yaml
Type: System.Drawing.Bitmap
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Percent
The size of the output bitmap relative to the original size.

```yaml
Type: System.Int32
Parameter Sets: Percentage
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Width
The width of the resized bitmap.

```yaml
Type: System.Int32
Parameter Sets: ExactSize
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Height
The height of the resized bitmap.

```yaml
Type: System.Int32
Parameter Sets: ExactSize
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -KeepAspectRatio
Keep the aspect ratio.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: ExactSize
Aliases:

Required: False
Position: 4
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
