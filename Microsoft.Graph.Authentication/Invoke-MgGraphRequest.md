---
external help file: Microsoft.Graph.Authentication.dll-Help.xml
Module Name: Microsoft.Graph.Authentication
online version: https://docs.microsoft.com/en-us/graph/permissions-reference
schema: 2.0.0
---

# Invoke-MgGraphRequest

## SYNOPSIS


## SYNTAX

```
Invoke-MgGraphRequest [[-Method] <GraphRequestMethod>] [-Uri] <Uri> [[-Body] <Object>]
 [[-Headers] <IDictionary>] [[-OutputFilePath] <String>] [-InferOutputFileName] [[-InputFilePath] <String>]
 [-PassThru] [[-Token] <SecureString>] [-SkipHeaderValidation] [[-ContentType] <String>]
 [[-Authentication] <GraphRequestAuthenticationType>] [[-SessionVariable] <String>]
 [[-ResponseHeadersVariable] <String>] [[-StatusCodeVariable] <String>] [-SkipHttpErrorCheck]
 [[-GraphRequestSession] <GraphRequestSession>] [[-UserAgent] <String>] [[-OutputType] <OutputType>] [-Break]
 [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell
PS C:\> 
```



## PARAMETERS

### -Authentication
Graph Authentication Type

```yaml
Type: Microsoft.Graph.PowerShell.Authentication.Models.GraphRequestAuthenticationType
Parameter Sets: (All)
Aliases:
Accepted values: Default, UserProvidedToken

Required: False
Position: 12
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body
Request Body.
Required when Method is Post or Patch

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByValue)
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
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContentType
Custom Content Type

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 11
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GraphRequestSession
Custom Graph Request Session

```yaml
Type: Microsoft.Graph.PowerShell.Authentication.Helpers.GraphRequestSession
Parameter Sets: (All)
Aliases:

Required: False
Position: 17
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Headers
Optional Custom Headers

```yaml
Type: System.Collections.IDictionary
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InferOutputFileName
Infer output filename

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputFilePath
Input file to send in the request

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Method
Http Method

```yaml
Type: Microsoft.Graph.PowerShell.Authentication.Models.GraphRequestMethod
Parameter Sets: (All)
Aliases:
Accepted values: GET, POST, PUT, PATCH, DELETE

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputFilePath
Output file where the response body will be saved

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputType
Output Type to return to the caller

```yaml
Type: Microsoft.Graph.PowerShell.Authentication.Models.OutputType
Parameter Sets: (All)
Aliases:
Accepted values: HashTable, PSObject, HttpResponseMessage, Json

Required: False
Position: 19
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Indicates that the cmdlet returns the results, in addition to writing them to a file.
Only valid when the OutFile parameter is also used.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResponseHeadersVariable
Response Headers Variable

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: RHV

Required: False
Position: 14
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SessionVariable
Specifies a web request session.
Enter the variable name, including the dollar sign ($).You can't use the SessionVariable and GraphRequestSession parameters in the same command.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: SV

Required: False
Position: 13
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkipHeaderValidation
Add headers to Request Header collection without validation

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkipHttpErrorCheck
Skip Checking Http Errors

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 16
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StatusCodeVariable
Response Status Code Variable

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 15
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Token
OAuth or Bearer Token to use instead of already acquired token

```yaml
Type: System.Security.SecureString
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Uri
Uri to call can be segments such as /beta/me or fully qualified https://graph.microsoft.com/beta/me

```yaml
Type: System.Uri
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserAgent
Custom User Specified User Agent

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 18
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Object

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
