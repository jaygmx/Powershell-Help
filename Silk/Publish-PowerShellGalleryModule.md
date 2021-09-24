---
external help file: Silk-help.xml
Module Name: Silk
online version: https://bitbucket.org/Swyter/bitbucket-curl-upload-to-repo-downloads
schema: 2.0.0
---

# Publish-PowerShellGalleryModule

## SYNOPSIS
Publishes a module to the PowerShell gallery.

## SYNTAX

```
Publish-PowerShellGalleryModule [-ManifestPath] <String> [-ModulePath] <String> [-ReleaseNotesPath] <String>
 [[-Name] <String>] [[-ApiKey] <String>] [-LicenseUri] <String> [[-Tags] <String[]>] [[-ProjectUri] <String>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The \`Publish-PowerShellGalleryModule\` functin publishes a module to the PowerShell Gallery.
If the given version of the module already exists in the Gallery, a warning is written and no other work is done.

If you don't supply a PowerShell Gallery API key via the \`ApiKey\` parameter, you'll be prompted for it.

Returns a \`PSGetItemInfo\` object if the module gets published (the object returned by the \`Find-Module\` cmdlet).
If the version of the module already exists in the Gallery, you'll get a warning that the module has already been published.

This function requires the \`PowerShellGet\` module.
If it isn't available, you'll get an error.

## EXAMPLES

### EXAMPLE 1
```
Publish-PowerShellGalleryModule -Name 'Carbon' -Version '2.0.0' -LicenseUri ''http://www.apache.org/licenses/LICENSE-2.0'
```

## PARAMETERS

### -ManifestPath
Path to the module's manifest.

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

### -ModulePath
The path to the module.

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

### -ReleaseNotesPath
The release notes.

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

### -Name
The name of the module being published.
Defaults to the name in the module manifest.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApiKey
The API key for the PowerShell Gallery.

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

### -LicenseUri
The URL to the module's license.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tags
Any tags for the module.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectUri
The URL to the project's home page.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
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

### PSGetItemInfo
## NOTES

## RELATED LINKS
