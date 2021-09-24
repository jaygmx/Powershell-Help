---
external help file: AdminToolbox.Office365-help.xml
Module Name: AdminToolbox.Office365
online version:
schema: 2.0.0
---

# New-AuthPolicy

## SYNOPSIS

## SYNTAX

```
New-AuthPolicy [<CommonParameters>]
```

## DESCRIPTION
Used to secure Exchange Online Authentication by creating authentication policies

Use of Modern Authentication Only is important for securing against Password Spray Attacks.
New attacks on Basic authentication allow for taking control of an Exchange Online account by simply sending a malicious link to a target.

Authentication Policies that are created are named...
"Modern Auth Only"
"Basic Auth Allowed"

## EXAMPLES

### EXAMPLE 1
```
Creates two Authentication Policies. One Basic and One Modern.
```

Set-AuthPolicy -CreatePolicies

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Requires the Exchange Online module be installed, imported, and Connected.

## RELATED LINKS

[Get-AuthPolicy
Set-AuthPolicy]()

