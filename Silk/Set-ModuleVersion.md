---
external help file: Silk-help.xml
Module Name: Silk
online version: https://bitbucket.org/Swyter/bitbucket-curl-upload-to-repo-downloads
schema: 2.0.0
---

# Set-ModuleVersion

## SYNOPSIS
Updates a module's version.

## SYNTAX

```
Set-ModuleVersion [-ManifestPath] <String> [[-SolutionPath] <String>] [[-AssemblyInfoPath] <String>]
 [[-ReleaseNotesPath] <String>] [[-NuspecPath] <String>] [[-Version] <Version>] [[-PreReleaseVersion] <String>]
 [[-BuildMetadata] <String>] [<CommonParameters>]
```

## DESCRIPTION


## EXAMPLES

### Example 1
```powershell

```



## PARAMETERS

### -ManifestPath
The path to the module's manifest.

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

### -SolutionPath
The path to the module's manifest.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AssemblyInfoPath
Path to an C# file to update with the assembly version.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReleaseNotesPath
Path to a release notes file.

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

### -NuspecPath
Path to the module's Nuspec file.

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

### -Version
The version to build.
If not provided, pulled from the module's manifest.

```yaml
Type: System.Version
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PreReleaseVersion
The pre-release version, e.g.
alpha.39, rc.1, etc.

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

### -BuildMetadata
Build metadata.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
