---
external help file: Firewall-Manager-help.xml
Module Name: Firewall-Manager
online version:
schema: 2.0.0
---

# Export-FirewallRules

## SYNOPSIS
Exports firewall rules to a CSV or JSON file.

## SYNTAX

```
Export-FirewallRules [[-Name] <Object>] [[-CSVFile] <Object>] [-JSON] [[-PolicyStore] <String>] [-Inbound]
 [-Outbound] [-Enabled] [-Disabled] [-Block] [-Allow]
```

## DESCRIPTION
Exports firewall rules to a CSV or JSON file.
Local and policy based rules will be given out.
CSV files are semicolon separated (Beware!
Excel is not friendly to CSV files).
All rules are exported by default, you can filter with parameter -Name, -Inbound, -Outbound,
-Enabled, -Disabled, -Allow and -Block.

## EXAMPLES

### EXAMPLE 1
```
Export-FirewallRules
Exports all firewall rules to the CSV file FirewallRules.csv in the current directory.
```

### EXAMPLE 2
```
Export-FirewallRules -Inbound -Allow
Exports all inbound and allowing firewall rules to the CSV file FirewallRules.csv in the current directory.
```

### EXAMPLE 3
```
Export-FirewallRules snmp* SNMPRules.json -json
Exports all SNMP firewall rules to the JSON file SNMPRules.json.
```

## PARAMETERS

### -Name
Display name of the rules to be processed.
Wildcard character * is allowed.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: *
Accept pipeline input: False
Accept wildcard characters: False
```

### -CSVFile
Output file

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JSON
Output in JSON instead of CSV format

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
Store from which the rules are retrieved (default: ActiveStore).
Allowed values are PersistentStore, ActiveStore (the resultant rule set of all sources), localhost,
a computer name, \<domain.fqdn.com\>\\\<GPO_Friendly_Name\>, RSOP and others depending on the environment.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: ActiveStore
Accept pipeline input: False
Accept wildcard characters: False
```

### -Inbound
Export inbound rules

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

### -Outbound
Export outbound rules

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

### -Enabled
Export enabled rules

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

### -Disabled
Export disabled rules

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

### -Block
Export blocking rules

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

### -Allow
Export allowing rules

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

## INPUTS

## OUTPUTS

## NOTES
Author: Markus Scholtes
Version: 1.1.0
Build date: 2020/12/12

## RELATED LINKS
