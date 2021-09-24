---
external help file: Microsoft.Graph.Reports-help.xml
Module Name: Microsoft.Graph.Reports
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.reports/get-mgreportsharepointsiteusagedetail204b
schema: 2.0.0
---

# Get-MgReportSharePointSiteUsageDetail204B

## SYNOPSIS
Invoke function getSharePointSiteUsageDetail

## SYNTAX

### Get (Default)
```
Get-MgReportSharePointSiteUsageDetail204B -Period <String> -OutFile <String> [-Break]
 [-HttpPipelineAppend <SendAsyncStep[]>] [-HttpPipelinePrepend <SendAsyncStep[]>] [-PassThru] [-Proxy <Uri>]
 [-ProxyCredential <PSCredential>] [-ProxyUseDefaultCredentials] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgReportSharePointSiteUsageDetail204B -InputObject <IReportsIdentity> -OutFile <String> [-Break]
 [-HttpPipelineAppend <SendAsyncStep[]>] [-HttpPipelinePrepend <SendAsyncStep[]>] [-PassThru] [-Proxy <Uri>]
 [-ProxyCredential <PSCredential>] [-ProxyUseDefaultCredentials] [<CommonParameters>]
```

## DESCRIPTION
Invoke function getSharePointSiteUsageDetail

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```



## PARAMETERS

### -Period
Usage: period={period}

```yaml
Type: System.String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IReportsIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OutFile
Path to write output file to

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Break
Wait for .NET debugger to attach

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

### -HttpPipelineAppend
SendAsync Pipeline Steps to be appended to the front of the pipeline

```yaml
Type: Microsoft.Graph.PowerShell.Runtime.SendAsyncStep[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HttpPipelinePrepend
SendAsync Pipeline Steps to be prepended to the front of the pipeline

```yaml
Type: Microsoft.Graph.PowerShell.Runtime.SendAsyncStep[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

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

### -Proxy
The URI for the proxy server to use

```yaml
Type: System.Uri
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProxyCredential
Credentials for a proxy server to use for the remote call

```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProxyUseDefaultCredentials
Use the default credentials for the proxy

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IReportsIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IReportsIdentity\>: Identity Parameter
  \[ApplicationSignInDetailedSummaryId \<String\>\]: key: id of applicationSignInDetailedSummary
  \[CredentialUserRegistrationDetailsId \<String\>\]: key: id of credentialUserRegistrationDetails
  \[Date \<DateTime?\>\]: Usage: date={date}
  \[DeviceManagementCachedReportConfigurationId \<String\>\]: key: id of deviceManagementCachedReportConfiguration
  \[DeviceManagementExportJobId \<String\>\]: key: id of deviceManagementExportJob
  \[DeviceManagementReportScheduleId \<String\>\]: key: id of deviceManagementReportSchedule
  \[DirectoryAuditId \<String\>\]: key: id of directoryAudit
  \[EndDateTime \<DateTime?\>\]: Usage: endDateTime={endDateTime}
  \[Filter \<String\>\]: Usage: filter={filter}
  \[GroupId \<String\>\]: Usage: groupId={groupId}
  \[IncludedUserRoles \<String\>\]: Usage: includedUserRoles={includedUserRoles}
  \[IncludedUserTypes \<String\>\]: Usage: includedUserTypes={includedUserTypes}
  \[Period \<String\>\]: Usage: period={period}
  \[PrintUsageByPrinterId \<String\>\]: key: id of printUsageByPrinter
  \[PrintUsageByUserId \<String\>\]: key: id of printUsageByUser
  \[PrinterId \<String\>\]: Usage: printerId={printerId}
  \[ProvisioningObjectSummaryId \<String\>\]: key: id of provisioningObjectSummary
  \[RestrictedSignInId \<String\>\]: key: id of restrictedSignIn
  \[SignInId \<String\>\]: key: id of signIn
  \[Skip \<Int32?\>\]: Usage: skip={skip}
  \[SkipToken \<String\>\]: Usage: skipToken={skipToken}
  \[StartDateTime \<DateTime?\>\]: Usage: startDateTime={startDateTime}
  \[Top \<Int32?\>\]: Usage: top={top}
  \[UserCredentialUsageDetailsId \<String\>\]: key: id of userCredentialUsageDetails
  \[UserId \<String\>\]: Usage: userId={userId}

## RELATED LINKS

[https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.reports/get-mgreportsharepointsiteusagedetail204b](https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.reports/get-mgreportsharepointsiteusagedetail204b)

