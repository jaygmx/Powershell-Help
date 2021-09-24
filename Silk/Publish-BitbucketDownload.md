---
external help file: Silk-help.xml
Module Name: Silk
online version: https://bitbucket.org/Swyter/bitbucket-curl-upload-to-repo-downloads
schema: 2.0.0
---

# Publish-BitbucketDownload

## SYNOPSIS
Creates and publishes a ZIP file to Bitbucket so it is available on a project's download page.

## SYNTAX

```
Publish-BitbucketDownload [[-Credential] <PSCredential>] [-Username] <String> [-ProjectName] <String>
 [-Path] <String[]> [-ManifestPath] <String> [<CommonParameters>]
```

## DESCRIPTION
The \`Publish-BitbucketDownload\` function creates a ZIP file and publishes it to a repository so it is availabe on a project's download page.
If the file already exists on Bitbucket, nothing is uploaded.

## EXAMPLES

### Example 1
```powershell
PS C:\> 
```

{{ Add example description here }}

## PARAMETERS

### -Credential
The Bitbucket credentials to use.

```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Username
The account of the project you're uploading a file to.

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

### -ProjectName
The name of the project you're uploading a file to.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
The paths to the files and directories to include in the ZIP file.
All files and sub-directories under directory are added.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManifestPath
The path to the manifest of the module being published.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 5
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

[https://bitbucket.org/Swyter/bitbucket-curl-upload-to-repo-downloads](https://bitbucket.org/Swyter/bitbucket-curl-upload-to-repo-downloads)

