---
external help file: AdminToolbox.Networking-help.xml
Module Name: AdminToolbox.Networking
online version:
schema: 2.0.0
---

# Invoke-NetworkScan

## SYNOPSIS

## SYNTAX

```
Invoke-NetworkScan [-CIDR] <String> [-DeepScan] [-SkipMac] [-Threads <String>] [<CommonParameters>]
```

## DESCRIPTION
Get Hostnames, IPAddresses, Open Ports, Mac Addresses, and Mac Vendors.

Mac resolution only works on locally attached networks.

## EXAMPLES

### EXAMPLE 1
```
Get details for all devices on the local subnet and sort by their OUI
```

Invoke-NetworkScan -CIDR 192.168.0.0/24 | Sort-Object Vendor

### EXAMPLE 2
```
Perform a more thorough port scan and output to gridview
```

Invoke-NetworkScan -CIDR 192.168.0.0/24 -DeepScan | Out-GridView

## PARAMETERS

### -CIDR
A CIDR Range to search.
ex: 192.168.0.0/24

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeepScan
Ports 21, 22, 23, 80, 443, 3389, 9100 are normally scanned.
Use DeepScan to get open ports for 21, 22, 23, 25, 53, 67, 80, 139, 389, 443, 445, 902, 3389, 9100.

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

### -SkipMac


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

### -Threads
Specify the number of threads that run on the port scan.
Default is 64

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 64
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Does not work in Powershell Core

## RELATED LINKS

[Invoke-PSipcalc https://www.powershellgallery.com/packages/PSnmap
Invoke-PSNmap https://www.powershellgallery.com/packages/PSnmap]()

