---
external help file: ImportExcel-help.xml
Module Name:
online version:
schema: 2.0.0
---

# Select-Worksheet

## SYNOPSIS
Sets the selected tab in an Excel workbook to be the chosen sheet and unselects all the others.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Select-Worksheet [-ExcelPackage] <ExcelPackage> [-WorksheetName <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Select-Worksheet -ExcelWorkbook <ExcelWorkbook> [-WorksheetName <String>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Select-Worksheet -ExcelWorksheet <ExcelWorksheet> [<CommonParameters>]
```

## DESCRIPTION
Sometimes when a sheet is added we want it to be the active sheet, sometimes we want the active sheet to be left as it was.
Select-Worksheet exists to change which sheet is the selected tab when Excel opens the file.

## EXAMPLES

### EXAMPLE 1
```
PS\> Select-Worksheet -ExcelWorkbook $ExcelWorkbook -WorksheetName "NewSheet"
```

$ExcelWorkbook holds a workbook object containing a sheet named "NewSheet"; This sheet will become the \[only\] active sheet in the workbook

### EXAMPLE 2
```
PS\>  Select-Worksheet -ExcelPackage $Pkg -WorksheetName "NewSheet2"
```

$pkg holds an Excel Package, whose workbook contains a sheet named "NewSheet2" This sheet will become the \[only\] active sheet in the workbook.

### EXAMPLE 3
```
PS\> Select-Worksheet -ExcelWorksheet $ws
```

$ws holds an Excel worksheet which will become the \[only\] active sheet in its workbook.

## PARAMETERS

### -ExcelPackage
An object representing an ExcelPackage.

```yaml
Type: ExcelPackage
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ExcelWorkbook
An Excel workbook to which the Worksheet will be added - a package contains one Workbook so you can use workbook or package as it suits.

```yaml
Type: ExcelWorkbook
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WorksheetName
The name of the worksheet "Sheet1" by default.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExcelWorksheet
An object representing an Excel worksheet.

```yaml
Type: ExcelWorksheet
Parameter Sets: UNNAMED_PARAMETER_SET_3
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

## OUTPUTS

## NOTES
*

## RELATED LINKS
