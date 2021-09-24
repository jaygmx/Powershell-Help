---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# New-HashObject

## SYNOPSIS
Create a PSObject from a dictionary such as a hashtable.

## SYNTAX

```
New-HashObject
```

## DESCRIPTION
Create a PSObject from a dictionary such as a hashtable. 
The keys-value
pairs are turned into NoteProperties.

## EXAMPLES

### EXAMPLE 1
```
$ht = @{fname='John';lname='Doe';age=42}; $ht | New-HashObject
Creates a hashtable in $ht and then converts that into a PSObject.
```

## PARAMETERS

## INPUTS

## OUTPUTS

## NOTES
Aliases:  nho

## RELATED LINKS
