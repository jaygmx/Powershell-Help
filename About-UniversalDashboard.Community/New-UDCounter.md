---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://github.com/ironmansoftware/universal-dashboard/blob/master/src/UniversalDashboard/Help/New-UDCounter.md
schema: 2.0.0
---

# New-UDCounter

## SYNOPSIS
Creates a simple counter.

## SYNTAX

```
New-UDCounter [-ArgumentList <Object[]>] [-AutoRefresh] [-BackgroundColor <DashboardColor>]
 [-Endpoint <ScriptBlock>] [-FontColor <DashboardColor>] [-Format <String>] [<CommonParameters>]
```

## DESCRIPTION
Creates a simple counter.
The counter number can be formatted using Numeral formats.
An icon can also be displayed with the Icon property.

## EXAMPLES

### Counter
```
New-UDCounter -Title "Total Bytes Downloaded" -AutoRefresh -RefreshInterval 3 -Format '0.00b' -Icon cloud_download -Endpoint {
	Get-Random -Minimum 0 -Maximum 100000000 | ConvertTo-Json
}
```

Outputs a random number as a counter.
Formats the number into KB, MB or TB depending on the size of the number returned.
Puts the cloud_download icon in the background.

## PARAMETERS

### -ArgumentList
Arguments to pass to the endpoint.
They will be available via the $ArgumentList variable.

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AutoRefresh
Enables auto refresh for this component.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackgroundColor
Background color of the panel.

```yaml
Type: DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Endpoint
The endpoint that is called on the server to get data for the counter.
The data should be piped to ConvertTo-Json before returning from this cmdlet.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontColor
The font color.

```yaml
Type: DashboardColor
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Format
The Numeral.js format for the counter.
See http://numeraljs.com/ for more information.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
