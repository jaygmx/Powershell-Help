---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Export-Bitmap

## SYNOPSIS
PSCX Cmdlet: Exports bitmap objects to various formats.

## SYNTAX

```
Export-Bitmap [-Path] <String> [[-Format] <BitmapFormat>] [[-Quality] <Int32>] [-PassThru] [-Bitmap] <Bitmap>
 [<CommonParameters>]
```

## DESCRIPTION
Exports a bitmap object to a specified file format.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
$bmp = (Import-Bitmap test.bmp | Resize-Bitmap -Perc 10);
              Export-Bitmap $bmp thumb.jpg Jpeg 50
```

Resizes the bitmap to 10% of its original size and saves it
                in a JPEG file with quality level 50.

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

### -Path
Specifies the path to the file that will be created.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
@{Text=}

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Format
Specifies the file format.
Supported values are:
              Bmp, Gif, Jpeg, Png, Tiff.

```yaml
Type: Pscx.Commands.Drawing.BitmapFormat
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: Jpeg
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Quality
Specifies the JPEG compression level.

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 75
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
