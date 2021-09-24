---
external help file: Silk-help.xml
Module Name: Silk
online version: https://bitbucket.org/Swyter/bitbucket-curl-upload-to-repo-downloads
schema: 2.0.0
---

# Publish-NuGetPackage

## SYNOPSIS
Creates and publishes a NuGet package to nuget.org.

## SYNTAX

```
Publish-NuGetPackage [-NupkgPath] <String> [[-ApiKey] <Object>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -NupkgPath
The path to the module manifest of the module you want to publish.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApiKey
The API key(s) to use.
To supply multiple API keys, use a hashtable where each key is a repository server name and the value is the API key for that repository.
For example,

@{ 'nuget.org' = '395edfa5-652f-4598-868e-c0a73be02c84' }

If not specified, you'll be prompted for it.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
