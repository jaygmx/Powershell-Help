---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# QuoteString

## SYNOPSIS
Creates a string from each parameter by concatenating each item using $OFS as the separator.

## SYNTAX

```
QuoteString
```

## DESCRIPTION
Creates a string from each parameter by concatenating each item using $OFS as the separator.

## EXAMPLES

### EXAMPLE 1
```
QuoteString $a $b $c
This is the equivalent of "$a $b $c".
```

### EXAMPLE 2
```
qs $a $b $c
This is the equivalent of "$a $b $c".  Same example as above but using the alias for QuoteString.
```

## PARAMETERS

## INPUTS

## OUTPUTS

## NOTES
Aliases:  qs

## RELATED LINKS
