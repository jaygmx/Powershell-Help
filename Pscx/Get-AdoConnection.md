---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-AdoConnection

## SYNOPSIS
PSCX Cmdlet: Create an ADO connection to any database supported by .NET on the current machine.
You can enumerate available ADO.NET Data Providers with the Get-AdoDataProvider Cmdlet.

## SYNTAX

### string (Default)
```
Get-AdoConnection [-ProviderName] <String> [-ConnectionString] <String> [<CommonParameters>]
```

### properties
```
Get-AdoConnection [-ProviderName] <String> [-ConnectionProperties] <Hashtable> [<CommonParameters>]
```

### simple
```
Get-AdoConnection [-ProviderName] <String> [-Server <String>] [-UserName <String>] [-Password <String>]
 [-Database <String>] [<CommonParameters>]
```

## DESCRIPTION
Create an ADO connection to any database supported by .NET on the current machine.
You can enumerate available ADO.NET Data Providers with the Get-AdoDataProvider Cmdlet.Data connections to supported providers are constructed using provider-agnostic common parameters like Server, Username, Password etc.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```

```

## PARAMETERS

### -ProviderName
@{Text=}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ConnectionProperties
@{Text=}

```yaml
Type: System.Collections.Hashtable
Parameter Sets: properties
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectionString
@{Text=}

```yaml
Type: System.String
Parameter Sets: string
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Database
@{Text=}

```yaml
Type: System.String
Parameter Sets: simple
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Password
@{Text=}

```yaml
Type: System.String
Parameter Sets: simple
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Server
@{Text=}

```yaml
Type: System.String
Parameter Sets: simple
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserName
@{Text=}

```yaml
Type: System.String
Parameter Sets: simple
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
