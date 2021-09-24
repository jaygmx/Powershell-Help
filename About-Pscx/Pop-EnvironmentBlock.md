---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Pop-EnvironmentBlock

## SYNOPSIS
PSCX Cmdlet: Pops the topmost environment block.

## SYNTAX

```
Pop-EnvironmentBlock [<CommonParameters>]
```

## DESCRIPTION
Pops the environment block and restores the state of all environment variables to the values stored in the environment block.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
C:\> Pop-EnvironmentBlock
```

Restores the current set of environment variables from the set at the top of the environment block stack.

## PARAMETERS

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

[Push-EnvironmentBlock]()

