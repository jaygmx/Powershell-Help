---
external help file: 7Zip4PowerShell.dll-Help.xml
Module Name: 7Zip4Powershell
online version:
schema: 2.0.0
---

# Get-7ZipInformation

## SYNOPSIS


## SYNTAX

### NoPassword (Default)
```
Get-7ZipInformation [-ArchiveFileName] <String[]> [<CommonParameters>]
```

### PlainPassword
```
Get-7ZipInformation [-ArchiveFileName] <String[]> [-Password <String>] [<CommonParameters>]
```

### SecurePassword
```
Get-7ZipInformation [-ArchiveFileName] <String[]> [-SecurePassword <SecureString>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -ArchiveFileName
The full file name of the archive

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Password


```yaml
Type: System.String
Parameter Sets: PlainPassword
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SecurePassword


```yaml
Type: System.Security.SecureString
Parameter Sets: SecurePassword
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

### System.String[]

## OUTPUTS

### SevenZip4PowerShell.ArchiveInformation

## NOTES

## RELATED LINKS
