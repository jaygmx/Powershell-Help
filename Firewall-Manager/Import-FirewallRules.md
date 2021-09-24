---
external help file: Firewall-Manager-help.xml
Module Name: Firewall-Manager
online version:
schema: 2.0.0
---

# Import-FirewallRules

## SYNOPSIS
Imports firewall rules from a CSV or JSON file.

## SYNTAX

```
Import-FirewallRules [[-CSVFile] <Object>] [-JSON] [[-PolicyStore] <String>]
```

## DESCRIPTION
Imports firewall rules from with Export-FirewallRules generated CSV or JSON files.
CSV files have to
be separated with semicolons.
Existing rules with same display name will be overwritten.

## EXAMPLES

### EXAMPLE 1
```
Import-FirewallRules
Imports all firewall rules in the CSV file FirewallRules.csv in the current directory.
```

### EXAMPLE 2
```
Import-FirewallRules WmiRules.json -json
Imports all firewall rules in the JSON file WmiRules.json.
```

## PARAMETERS

### -CSVFile
Input file

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JSON
Input in JSON instead of CSV format

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

### -PolicyStore
Store to which the rules are written (default: PersistentStore).
Allowed values are PersistentStore, ActiveStore (the resultant rule set of all sources), localhost,
a computer name, \<domain.fqdn.com\>\\\<GPO_Friendly_Name\> and others depending on the environment.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: PersistentStore
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
Author: Markus Scholtes
Version: 1.1.0
Build date: 2020/12/12

## RELATED LINKS
