---
external help file: module-help.xml
Module Name: PSOneTools
online version: https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Get-PSOneToken.ps1
schema: 2.0.0
---

# Get-PSOneToken

## SYNOPSIS
Parses a PowerShell Script (*.ps1, *.psm1, *.psd1) and returns the token

## SYNTAX

### Path (Default)
```
Get-PSOneToken -Path <String> [-TokenKind <TokenKind[]>] [-TokenFlag <TokenFlags[]>] [-IncludeNestedToken]
 [<CommonParameters>]
```

### ScriptBlock
```
Get-PSOneToken -ScriptBlock <ScriptBlock> [-TokenKind <TokenKind[]>] [-TokenFlag <TokenFlags[]>]
 [-IncludeNestedToken] [<CommonParameters>]
```

### Code
```
Get-PSOneToken -Code <String> [-TokenKind <TokenKind[]>] [-TokenFlag <TokenFlags[]>] [-IncludeNestedToken]
 [<CommonParameters>]
```

## DESCRIPTION
Invokes the advanced PowerShell Parser and returns tokens and syntax errors

## EXAMPLES

### EXAMPLE 1
```
Get-PSOneToken -Path c:\test.ps1
Parses the content of c:\test.ps1 and returns tokens and syntax errors
```

### EXAMPLE 2
```
Get-ChildItem -Path $home -Recurse -Include *.ps1,*.psm1,*.psd1 -File |
Get-PSOneToken |
Out-GridView
```

parses all PowerShell files found anywhere in your user profile

### EXAMPLE 3
```
Get-ChildItem -Path $home -Recurse -Include *.ps1,*.psm1,*.psd1 -File |
Get-PSOneToken |
Where-Object Errors
```

parses all PowerShell files found anywhere in your user profile
and returns only those files that contain syntax errors

## PARAMETERS

### -Path
Path to PowerShell script file
can be a string or any object that has a "Path" 
or "FullName" property:

```yaml
Type: System.String
Parameter Sets: Path
Aliases: FullName

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ScriptBlock
PowerShell Code as ScriptBlock

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: ScriptBlock
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Code
PowerShell Code as String

```yaml
Type: System.String
Parameter Sets: Code
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TokenKind
the kind of token requested.
If neither TokenKind nor TokenFlag is requested, 
a full tokenization occurs

```yaml
Type: System.Management.Automation.Language.TokenKind[]
Parameter Sets: (All)
Aliases:
Accepted values: Unknown, Variable, SplattedVariable, Parameter, Number, Label, Identifier, Generic, NewLine, LineContinuation, Comment, EndOfInput, StringLiteral, StringExpandable, HereStringLiteral, HereStringExpandable, LParen, RParen, LCurly, RCurly, LBracket, RBracket, AtParen, AtCurly, DollarParen, Semi, AndAnd, OrOr, Ampersand, Pipe, Comma, MinusMinus, PlusPlus, DotDot, ColonColon, Dot, Exclaim, Multiply, Divide, Rem, Plus, Minus, Equals, PlusEquals, MinusEquals, MultiplyEquals, DivideEquals, RemainderEquals, Redirection, RedirectInStd, Format, Not, Bnot, And, Or, Xor, Band, Bor, Bxor, Join, Ieq, Ine, Ige, Igt, Ilt, Ile, Ilike, Inotlike, Imatch, Inotmatch, Ireplace, Icontains, Inotcontains, Iin, Inotin, Isplit, Ceq, Cne, Cge, Cgt, Clt, Cle, Clike, Cnotlike, Cmatch, Cnotmatch, Creplace, Ccontains, Cnotcontains, Cin, Cnotin, Csplit, Is, IsNot, As, PostfixPlusPlus, PostfixMinusMinus, Shl, Shr, Colon, QuestionMark, QuestionQuestionEquals, QuestionQuestion, QuestionDot, QuestionLBracket, Begin, Break, Catch, Class, Continue, Data, Define, Do, Dynamicparam, Else, ElseIf, End, Exit, Filter, Finally, For, Foreach, From, Function, If, In, Param, Process, Return, Switch, Throw, Trap, Try, Until, Using, Var, While, Workflow, Parallel, Sequence, InlineScript, Configuration, DynamicKeyword, Public, Private, Static, Interface, Enum, Namespace, Module, Type, Assembly, Command, Hidden, Base, Default

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TokenFlag
the kind of token requested.
If neither TokenKind nor TokenFlag is requested, 
a full tokenization occurs

```yaml
Type: System.Management.Automation.Language.TokenFlags[]
Parameter Sets: (All)
Aliases:
Accepted values: None, BinaryPrecedenceLogical, BinaryPrecedenceBitwise, BinaryPrecedenceComparison, BinaryPrecedenceCoalesce, BinaryPrecedenceAdd, BinaryPrecedenceMultiply, BinaryPrecedenceFormat, BinaryPrecedenceRange, BinaryPrecedenceMask, Keyword, ScriptBlockBlockName, BinaryOperator, UnaryOperator, CaseSensitiveOperator, TernaryOperator, SpecialOperator, AssignmentOperator, ParseModeInvariant, TokenInError, DisallowedInRestrictedMode, PrefixOrPostfixOperator, CommandName, MemberName, TypeName, AttributeName, CanConstantFold, StatementDoesntSupportAttributes

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeNestedToken
include nested token that are contained inside 
ExpandableString tokens

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

[https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Get-PSOneToken.ps1](https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Get-PSOneToken.ps1)

[https://powershell.one/powershell-internals/parsing-and-tokenization/advanced-tokenizer
https://github.com/TobiasPSP/Modules.PSOneTools/blob/master/PSOneTools/1.4/Get-PSOneToken.ps1]()

