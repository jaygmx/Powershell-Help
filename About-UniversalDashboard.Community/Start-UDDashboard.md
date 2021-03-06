---
external help file: UniversalDashboard.Community-help.xml
Module Name:
online version: https://go.microsoft.com/fwlink/?LinkID=217032
schema: 2.0.0
---

# Start-UDDashboard

## SYNOPSIS
Starts a dashboard defined by New-UDDashboard.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Start-UDDashboard [-AutoReload] [-Certificate <X509Certificate2>] [-CertificateFile <String>]
 [-CertificateFilePassword <SecureString>] [-Content <ScriptBlock>] [-DisableTelemetry]
 [-Endpoint <Endpoint[]>] [-Force] [-HttpsPort <Int32>] [-ListenAddress <IPAddress>] [-Name <String>]
 [-Port <Int32>] [-PublishedFolder <PublishedFolder[]>] [-UpdateToken <String>] [-Wait] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Start-UDDashboard [-AutoReload] [-Certificate <X509Certificate2>] [-CertificateFile <String>]
 [-CertificateFilePassword <SecureString>] [-Dashboard <Dashboard>] [-DisableTelemetry]
 [-Endpoint <Endpoint[]>] [-Force] [-HttpsPort <Int32>] [-ListenAddress <IPAddress>] [-Name <String>]
 [-Port <Int32>] [-PublishedFolder <PublishedFolder[]>] [-UpdateToken <String>] [-Wait] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Start-UDDashboard [-AutoReload] [-Certificate <X509Certificate2>] [-CertificateFile <String>]
 [-CertificateFilePassword <SecureString>] [-DisableTelemetry] [-Endpoint <Endpoint[]>] [-FilePath <String>]
 [-Force] [-HttpsPort <Int32>] [-ListenAddress <IPAddress>] [-Name <String>] [-Port <Int32>]
 [-PublishedFolder <PublishedFolder[]>] [-UpdateToken <String>] [-Wait] [<CommonParameters>]
```

## DESCRIPTION
Starts a dashboard defined by New-UDDashboard.

## EXAMPLES

### Example 1
```
PS C:\> Start-UDDashboard -Content {
	New-UDDashboard -Title "Groovy Dashboard" 
}
```

Starts a new dashboard based on the specified ScriptBlock with the title Groovy Dashboard on port 80.

### Example 2
```
PS C:\> $Dashboard = New-UDDashboard -Title "Groovy Dashboard" 
PS C:\> Start-UDDashboard -Dashboard $Dashboard -Port 1000
```

Starts a new dashboard based on the specified dashboard created by New-Dashboard with the title Groovy Dashboard on port 1000.

### Example 3
```
PS C:\> Start-UDDashboard -Name "MyDashboard" -Content {
	New-UDDashboard -Title "Groovy Dashboard" 
}
```

Starts a new dashboard with the name "MyDashboard".

## PARAMETERS

### -AutoReload
Reloads the dashboard automatically when changes are made to the script containing the dashboard.
The dashboard must be saved as a file.

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

### -Certificate
The certificate to use encrypt HTTPS traffic.
The webserver will listen on HTTPS.

```yaml
Type: X509Certificate2
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificateFile
The certificate file to use encrypt HTTPS traffic.
The webserver will listen on HTTPS.

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

### -CertificateFilePassword
The certificate file password to use encrypt HTTPS traffic.
The webserver will listen on HTTPS.

```yaml
Type: SecureString
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Content
A ScriptBlock that calls New-UDDashboard.

```yaml
Type: ScriptBlock
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Dashboard
The dashboard to start.
This dashboard is created with New-UDDashboard.

```yaml
Type: Dashboard
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisableTelemetry


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

### -Endpoint
An array of REST endpoints to expose with this dashboard.
They can be generated with New-UDEndpoint.

```yaml
Type: Endpoint[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FilePath
The path to a file that returns a dashboard.
This file should return a dashboard with New-UDDashboard.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Starts a dashboard and stops any dashboard running on the same port.

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

### -HttpsPort
The HTTPS port to listen on.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ListenAddress
The IP Addresses to listen on.

```yaml
Type: IPAddress
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Name of the dashboard.

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

### -Port
The port to use for the dashboard.
Defaults to 80.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PublishedFolder
A collection of published folders.
You can generate these folders with Publish-UDFolder.

```yaml
Type: PublishedFolder[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UpdateToken
A token used to authenticate update requests.

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

### -Wait
Blocks execution and waits for the web server to run.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### System.Object
## NOTES
*

## RELATED LINKS
