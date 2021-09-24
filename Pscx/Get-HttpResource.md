---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-HttpResource

## SYNOPSIS
PSCX Cmdlet: Gets an HTTP resource or optionally the headers associated with the resource.

## SYNTAX

### Authenticated (Default)
```
Get-HttpResource [-AcceptHeader <String>] [-HeadersOnly] [-ReadCount <Int64>] [-Encoding <EncodingParameter>]
 [-ReadWriteTimeout <TimeSpan>] [-Url] <Uri> [-Credential <PSCredential>] [-Proxy <IWebProxy>]
 [-Timeout <Int32>] [-UserAgent <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Anonymous
```
Get-HttpResource [-AcceptHeader <String>] [-HeadersOnly] [-ReadCount <Int64>] [-Encoding <EncodingParameter>]
 [-ReadWriteTimeout <TimeSpan>] [-Url] <Uri> [-Anonymous] [-Proxy <IWebProxy>] [-Timeout <Int32>]
 [-UserAgent <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Gets an HTTP resource or optionally the headers associated with the resource.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
PS> Get-HttpResource http://blogs.msdn.com/powershell
```

Gets the contents of the above URL as a string.

### EXAMPLE 2
PS C:\\\>

```
PS> Get-HttpResource -headersOnly http://assets0.twitter.com/images/twitter_logo_header.png
          
          Name                           Value
          ----                           -----
          Content-Length                 6656
          Last-Modified                  Fri, 08 May 2009 21:40:51 GMT
          Expires                        Wed, 08 May 2019 19:54:41 GMT
          Server                         Apache
          Accept-Ranges                  bytes
          Content-Type                   image/png
          Cache-Control                  max-age=315360000
          Date                           Sun, 10 May 2009 19:54:41 GMT
          Connection                     close
```

Gets just the headers for the URL.

## PARAMETERS

### -Url
The url of the HTTP resource to get.

```yaml
Type: System.Uri
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -AcceptHeader
AcceptHeader allows you to specify which media type is preferred in response.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Null
Accept pipeline input: False
Accept wildcard characters: False
```

### -Anonymous
Use anonymous credentials when accessing the URL.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: Anonymous
Aliases:

Required: False
Position: Named
Default value: N/A
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
Credential to use when accessing the URL.

```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: Authenticated
Aliases:

Required: False
Position: Named
Default value: N/A
Accept pipeline input: False
Accept wildcard characters: False
```

### -Encoding
The encoding to use for string InputObjects. 
Valid values are: Byte, ASCII, UTF7, UTF8, UTF32, Unicode, BigEndianUnicode and Default.

```yaml
Type: Pscx.EncodingParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Byte will cause the result to be output as an array
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeadersOnly
Retrieves just the headers for the specified URL.
This option can be used as a light weight way to determine properties of certain URLs such as the size of an image.

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
Allows the proxy information to be customized for this request. 
Create and configure a new System.Net.WebProxy object to supply for this parameter.

```yaml
Type: System.Net.IWebProxy
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReadCount
ReadCount determines how many items of data are processed before sending down the pipeline.
An an item will be either a string or a byte (when -Encoding Byte) is used.
A value of 0 will cause the entire response to be sent as a single string or byte array. 
A value of 1 will cause each line or byte of the response to be sent down the pipeline.
A value of N, where N \> 1 will cause an array of strings or bytes of size N (or smaller) to be sent down the pipeline.

```yaml
Type: System.Int64
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReadWriteTimeout
Sets a time-out in milliseconds when reading from the stream of data in the response.

```yaml
Type: System.Nullable`1[System.TimeSpan]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 300,000 milliseconds (5 minutes)
Accept pipeline input: False
Accept wildcard characters: False
```

### -Timeout
Sets the time-out value in milliseconds for the GetResponse and GetRequestStream methods

```yaml
Type: System.Nullable`1[System.Int32]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 100,000 milliseconds (100 seconds)
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserAgent
The user agent string to use in the web request's header.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: PSCX_HttpResource_Cmdlet
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

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

### String
### Byte
### Hashtable
## NOTES

## RELATED LINKS
