---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Expand-PSOneToken.ps1
schema: 2.0.0
---

# Expand-PSOneToken

## SYNOPSIS
Expands all nested token from a token of type "StringExpandable"

## SYNTAX

### ExpandableString (Default)
```
Expand-PSOneToken [-StringExpandable] <StringExpandableToken> [<CommonParameters>]
```

### Token
```
Expand-PSOneToken [-Token] <Token> [<CommonParameters>]
```

## DESCRIPTION
Recursively emits all tokens embedded in a token of type "StringExpandable"
The original token is also emitted.

## EXAMPLES

### EXAMPLE 1
```
Get-PSOneToken -Code '"Hello $host"' -TokenKind StringExpandable | Expand-PSOneToken 
Emits all tokens, including the embedded (nested) tokens
```

## PARAMETERS

### -StringExpandable
binds a token of type "StringExpandableToken"

```yaml
Type: System.Management.Automation.Language.StringExpandableToken
Parameter Sets: ExpandableString
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Token
binds all tokens

```yaml
Type: System.Management.Automation.Language.Token
Parameter Sets: Token
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Expand-PSOneToken.ps1](https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Expand-PSOneToken.ps1)

[https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Expand-PSOneToken.ps1]()

