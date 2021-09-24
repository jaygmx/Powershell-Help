---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Push-EnvironmentBlock

## SYNOPSIS
PSCX Cmdlet: Pushes the current environment onto the environment block stack.

## SYNTAX

```
Push-EnvironmentBlock [-Description <String>] [<CommonParameters>]
```

## DESCRIPTION
Stores the state of all environment variables into an environment block and pushes that onto the environment block stack.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\> Push-EnvironmentBlock -Description "Before loading VS 2010 env vars"
```

## PARAMETERS

### -Description
@{Text=}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
*

## RELATED LINKS

[Add-PathVariable]()

[Get-PathVariable]()

[Set-PathVariable]()

[Pop-EnvironmentBlock]()

