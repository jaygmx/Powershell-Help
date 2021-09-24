---
external help file: Pscx.dll-Help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Get-TypeName

## SYNOPSIS
PSCX Cmdlet: Get-TypeName displays the typename of the input object.

## SYNTAX

```
Get-TypeName [-InputObject] <PSObject> [-FullName] [-PassThru] [<CommonParameters>]
```

## DESCRIPTION
Get-TypeName displays the typename of the input object.
Normally you would use Get-Member to
    determine this but if you are only interested in the type name
    this filter produces much less output. 
Also, since Get-Member
    accumulates multiple instances of the same type into a single output
    record for that type, you don't get any sense of how many objects of
    that type are traversing the pipeline. 
With Get-TypeName, you will
    see the type name of *every* object passed into it. 
NOTE: If you
    specify any arguments then all pipeline input is ignored.
This is
    due to the fact that PowerShell executes the Process function even
    if there isn't any input so it is impossible to distinguish between
    $null pipeline input and no pipeline input. 
NOTE: the type name is displayed
    directly to the host so that it doesn't interfere with pipeline operations.
    If you want the original object to pass thru, use the PassThru parameter.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
PS> Get-TypeName (Get-Date)
```

Displays the typename for the object returned by the Get-Date cmdlet.

### EXAMPLE 2
PS C:\\\>

```
PS> Get-Command Get-* | Get-TypeName
```

Displays the typename for each of the Get cmdlets.

### EXAMPLE 3
PS C:\\\>

```
PS> Get-TypeName $PSVersionTable
```

Displays the typename for each of the $PSVersionTable variable.

### EXAMPLE 4
PS C:\\\>

```
PS> $PSVersionTable | Get-TypeName -PassThru | Foreach {$_.PSVersion}
```

Stick Get-TypeName -PassThru in the middle of a pipeline to observe the object types in the pipeline.

## PARAMETERS

### -InputObject
The object whose typename you want to know.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: N/A
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -FullName
Displays the full type name.

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

### -PassThru
Outputs the original input object and writes the typename to the host.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### PSObject
## OUTPUTS

### PSObject
## NOTES

## RELATED LINKS
