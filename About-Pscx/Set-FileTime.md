---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Set-FileTime

## SYNOPSIS
PSCX Cmdlet: Sets a file or folder's created and last accessed/write times.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Set-FileTime [-Path] <String[]> [[-Time] <DateTime>] [-Accessed] [-Created] [-Force] [-Modified] [-PassThru]
 [-UseTimeFromFile <String>] [-Utc] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Set-FileTime [-LiteralPath] <String[]> [[-Time] <DateTime>] [-Accessed] [-Created] [-Force] [-Modified]
 [-PassThru] [-UseTimeFromFile <String>] [-Utc] [<CommonParameters>]
```

## DESCRIPTION
Sets a file or folder's created and last accessed/write times.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:PS> Set-FileTime foo.txt
```

Updates the LastWriteTime and LastAccessTime properties of the file foo.txt to the current local time.

### EXAMPLE 2
PS C:\\\>

```
C:PS> Set-FileTime foo.txt -Time ((get-date).AddDays(-14))
```

Updates the LastWriteTime and LastAccessTime properties of the file foo.txt to the current local time minus 14 days.

### EXAMPLE 3
PS C:\\\>

```
C:PS> Get-ChildItem . *.cs -r | Set-FileTime
```

Updates the LastWriteTime and LastAccessTime properties on all files with extension .CS in the current dir and below to the current local time.

### EXAMPLE 4
PS C:\\\>

```
C:PS> Get-ChildItem . *.cs -r | Set-FileTime -Modified
```

Updates only the LastWriteTime property on all files with extension .CS in the current dir and below to the current local time.

### EXAMPLE 5
PS C:\\\>

```
C:PS> Get-ChildItem . *.cs -r | Set-FileTime -UseTimeFromFile C:\boot.ini
```

Updates the LastWriteTime and LastAccessTime properties on all files with extension .CS in the current dir and below to the same time as the LastWriteTime of the file C:\boot.ini.

## PARAMETERS

### -LiteralPath
Specifies a path to the item.
The value of -LiteralPath is used exactly as it is typed.
No characters are interpreted as wildcards.
If the path includes escape characters, enclose it in single quotation marks.
Single quotation marks tell Windows PowerShell not to interpret any characters as escape sequences.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Specifies the path to the file to process.
Wildcard syntax is allowed.

```yaml
Type: String[]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### -Time
The time to use to set the access, created and modified times unless -Accessed, -Created and/or -Modified is specified, then only those times will be updated.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: The current system time
Accept pipeline input: False
Accept wildcard characters: False
```

### -Accessed
Update the accessed time. 
Created and modified time will not be updated unless also specified.
Parameter alias is SetAccessedTime.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
```

### -Created
Update the created time. 
Accessed and modified time will not be upated unless also specified.
Parameter alias is SetCreatedTime.

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

### -Force
Attempt to set the specified time even if the file is readonly.

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

### -Modified
Update the modified time. 
Accessed and created time will not be updated unless also specified.
Parameter alias is SetModifiedTime.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Passing the processing path to the next stage of the pipeline.

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

### -UseTimeFromFile
Use the date and time from the file at the specified path to set the access and/or write times.

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

### -Utc
Set the accessed, created and/or modified times as UTC times.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS
