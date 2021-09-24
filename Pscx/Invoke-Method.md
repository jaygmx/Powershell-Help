---
external help file: Pscx-help.xml
Module Name: Pscx
online version:
schema: 2.0.0
---

# Invoke-Method

## SYNOPSIS
Function to call a single method on an incoming stream of piped objects.

## SYNTAX

```
Invoke-Method -InputObject <Object> [-MethodName] <String> [-Arguments <Object[]>] [-Static]
 [<CommonParameters>]
```

## DESCRIPTION
Function to call a single method on an incoming stream of piped objects.
Methods can be static or instance and
arguments may be passed as an array or individually.

## EXAMPLES

### EXAMPLE 1
```
1..3 | invoke-method gettype
Calls GetType() on each incoming integer.
```

### EXAMPLE 2
```
dir *.txt | invoke-method moveto "c:\temp\"
Calls the MoveTo() method on all txt files in the current directory passing in "C:\Temp" as the destFileName.
```

## PARAMETERS

### -InputObject
The object to execute the named method on.
Accepts pipeline input.

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MethodName


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

### -Arguments
The arguments to pass to the named method, if any.

```yaml
Type: System.Object[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Static
The member name will be treated as a static method call on the incoming object.

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

## OUTPUTS

## NOTES
Aliases:  call

## RELATED LINKS
