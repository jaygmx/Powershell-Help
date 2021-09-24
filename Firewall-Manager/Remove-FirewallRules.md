---
external help file: Firewall-Manager-help.xml
Module Name: Firewall-Manager
online version:
schema: 2.0.0
---

# Remove-FirewallRules

## SYNOPSIS
Removes firewall rules according to a list in a CSV or JSON file.

## SYNTAX

```
Remove-FirewallRules [[-CSVFile] <Object>] [-JSON] [[-PolicyStore] <String>]
```

## DESCRIPTION
Removes firewall rules according to a with Export-FirewallRules generated list in a CSV or JSON file.
CSV files have to be separated with semicolons.
Only the field Name or - if Name is missing - DisplayName
is used, alle other fields can be omitted
anderen

## EXAMPLES

### EXAMPLE 1
```
Remove-FirewallRules
Removes all firewall rules according to a list in the CSV file FirewallRules.csv in the current directory.
```

### EXAMPLE 2
```
Remove-FirewallRules WmiRules.json -json
Removes all firewall rules according to the list in the JSON file WmiRules.json.
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
Store from which rules are removed (default: PersistentStore).
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
