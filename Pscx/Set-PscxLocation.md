---
external help file: Pscx-help.xml
Module Name: Pscx
online version: http://en.wikipedia.org/wiki/Less_(Unix)
schema: 2.0.0
---

# Set-PscxLocation

## SYNOPSIS
Set-PscxLocation function that tracks location history allowing easy navigation to previous locations.

## SYNTAX

### Path (Default)
```
Set-PscxLocation [[-Path] <String>] [-UnboundArguments <String[]>] [-PassThru] [-UseTransaction]
 [<CommonParameters>]
```

### LiteralPath
```
Set-PscxLocation [[-LiteralPath] <String>] [-UnboundArguments <String[]>] [-PassThru] [-UseTransaction]
 [<CommonParameters>]
```

## DESCRIPTION
Set-PscxLocation function that tracks location history allowing easy navigation to previous locations.
Set-PscxLocation maintains a backward and forward stack mechanism that can be navigated using "Set-PscxLocation -"
to go backwards in the stack and "Set-PscxLocation +" to go forwards in the stack. 
Executing "Set-PscxLocation"
without any parameters will display the current stack history. 

By default, the new location is echo'd to the host. 
If you want to suppress this set the preference 
variable in your profile e.g.
$Pscx:Preferences\['CD_EchoNewLocation'\] = $false. 

If you want to change your cd alias to use Set-PscxLocation, execute:
Set-Alias cd Set-PscxLocation -Option AllScope

## EXAMPLES

### EXAMPLE 1
```
set-alias cd Set-PscxLocation -Option AllScope; cd $pshome; cd -; cd +
This example changes location to the PowerShell install dir, then back to the original
location, than forward again to the PowerShell install dir.
```

### EXAMPLE 2
```
set-alias cd Set-PscxLocation -Option AllScope; cd ....
This example changes location up two levels from the current path.  You can use an arbitrary
number of periods to indicate how many levels you want to go up.  A single period "." indicates
the current location.  Two periods ".." indicate the current location's parent.  Three periods "..."
indicates the current location's parent's parent and so on.
```

### EXAMPLE 3
```
set-alias cd Set-PscxLocation -Option AllScope; cd
Executing CD without any parameters will cause it to display the current stack contents.
```

### EXAMPLE 4
```
set-alias cd Set-PscxLocation -Option AllScope; cd -0
Changes location to the very first (0th index) location in the stack. Execute CD without any parameters
to see all the paths, then execute CD -<number> to change location to that path.
```

### EXAMPLE 5
```
set-alias cd Set-PscxLocation -Option AllScope; $profile | cd
This example will change location to the parent location of $profile.
```

## PARAMETERS

### -Path
The path to change location to.

```yaml
Type: System.String
Parameter Sets: Path
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -LiteralPath
The literal path to change location to. 
This path can contain wildcard characters that
do not need to be escaped.

```yaml
Type: System.String
Parameter Sets: LiteralPath
Aliases: PSPath

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UnboundArguments
This parameter accumulates all the additional arguments and concatenates them to the Path
or LiteralPath parameter using a space separator. 
This allows you to cd to some paths containing
spaces without having to quote the path e.g.
'cd c:\program files'. 
Note that this doesn't always
work. 
For example, this following won't work: 'cd c:\program files (x86)'. 
This fails because
PowerShell tries to evaluate the contents of the expression '(x86)' which isn't a valid command name.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
If the PassThru switch is specified the object passed into the Set-PscxLocation function is also output
from the function. 
This allows the next pipeline stage to also operate on the object.

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

### -UseTransaction
Includes the command in the active transaction.
This parameter is valid only when a transaction
is in progress.
For more information, see about_Transactions. 
This parameter is not supported
in PowerShell Core.

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
This is a PSCX function.

## RELATED LINKS
