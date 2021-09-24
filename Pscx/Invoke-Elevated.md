---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Invoke-Elevated

## SYNOPSIS
Runs the specified command in an elevated context.

## SYNTAX

```
Invoke-Elevated
```

## DESCRIPTION
Runs the specified command in an elevated context. 
This is useful on Windows Vista
and Windows 7 when you run with a standard user token but can elevate to Admin when needed.

## EXAMPLES

### EXAMPLE 1
```
Invoke-Elevated
Opens a new PowerShell instance as admin.
```

### EXAMPLE 2
```
Invoke-Elevated Notepad C:\windows\system32\drivers\etc\hosts
Opens notepad elevated with the hosts file so that you can save changes to the file.
```

### EXAMPLE 3
```
Invoke-Elevated {gci c:\windows\temp | export-clixml tempdir.xml; exit}
Executes the scriptblock in an elevated PowerShell instance.
```

### EXAMPLE 4
```
Invoke-Elevated {gci c:\windows\temp | export-clixml tempdir.xml; exit} | %{$_.WaitForExit(5000)} | %{Import-Clixml tempdir.xml}
Executes the scriptblock in an elevated PowerShell instance, waits for that elevated process to execute, then
retrieves the results.
```

## PARAMETERS

## INPUTS

## OUTPUTS

## NOTES
Aliases:  su
Author:   Keith Hill

## RELATED LINKS
