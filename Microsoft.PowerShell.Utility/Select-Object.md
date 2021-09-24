---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
Module Name: Microsoft.PowerShell.Utility
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/select-object?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Select-Object

## SYNOPSIS
Selects objects or object properties.

## SYNTAX

### DefaultParameter (Default)
```
Select-Object [-InputObject <PSObject>] [[-Property] <Object[]>] [-ExcludeProperty <String[]>]
 [-ExpandProperty <String>] [-Unique] [-Last <Int32>] [-First <Int32>] [-Skip <Int32>] [-Wait]
 [<CommonParameters>]
```

### SkipLastParameter
```
Select-Object [-InputObject <PSObject>] [[-Property] <Object[]>] [-ExcludeProperty <String[]>]
 [-ExpandProperty <String>] [-Unique] [-SkipLast <Int32>] [<CommonParameters>]
```

### IndexParameter
```
Select-Object [-InputObject <PSObject>] [-Unique] [-Wait] [-Index <Int32[]>] [<CommonParameters>]
```

### SkipIndexParameter
```
Select-Object [-InputObject <PSObject>] [-Unique] [-SkipIndex <Int32[]>] [<CommonParameters>]
```

## DESCRIPTION
The \`Select-Object\` cmdlet selects specified properties of an object or set of objects.
It can also select unique objects, a specified number of objects, or objects in a specified position in an array.

To select objects from a collection, use the First , Last , Unique , Skip , and Index parameters.
To select object properties, use the Property parameter.
When you select properties, \`Select-Object\` returns new objects that have only the specified properties.

Beginning in Windows PowerShell 3.0, \`Select-Object\` includes an optimization feature that prevents commands from creating and processing objects that are not used.

When you include a \`Select-Object\` command with the First or Index parameters in a command pipeline, PowerShell stops the command that generates the objects as soon as the selected number of objects is generated, even when the command that generates the objects appears before the \`Select-Object\` command in the pipeline.
To turn off this optimizing behavior, use the Wait parameter.

## EXAMPLES

### Example 1: Select objects by property
```
Get-Process | Select-Object -Property ProcessName, Id, WS
```

### Example 2: Select objects by property and format the results
```
Get-Process Explorer | Select-Object -Property ProcessName -ExpandProperty Modules | Format-List

ProcessName       : explorer
ModuleName        : explorer.exe
FileName          : C:\WINDOWS\explorer.exe
BaseAddress       : 140697278152704
ModuleMemorySize  : 3919872
EntryPointAddress : 140697278841168
FileVersionInfo   : File:             C:\WINDOWS\explorer.exe
                    InternalName:     explorer
                    OriginalFilename: EXPLORER.EXE.MUI
                    FileVersion:      10.0.17134.1 (WinBuild.160101.0800)
                    FileDescription:  Windows Explorer
                    Product:          Microsoft Windows Operating System
                    ProductVersion:   10.0.17134.1
...
```

### Example 3: Select processes using the most memory
```
Get-Process | Sort-Object -Property WS | Select-Object -Last 5

Handles  NPM(K)    PM(K)      WS(K) VS(M)   CPU(s)     Id ProcessName
-------  ------    -----      ----- -----   ------     -- -----------
2866     320       33432      45764   203   222.41   1292 svchost
577      17        23676      50516   265    50.58   4388 WINWORD
826      11        75448      76712   188    19.77   3780 Ps
1367     14        73152      88736   216    61.69    676 Ps
1612     44        66080      92780   380   900.59   6132 INFOPATH
```

### Example 4: Select unique characters from an array
```
"a","b","c","a","a","a" | Select-Object -Unique

a
b
c
```

### Example 5: Select newest and oldest events in the event log
```
$a = Get-EventLog -LogName "Windows PowerShell"
$a | Select-Object -Index 0, ($A.count - 1)
```

### Example 6: Select all but the first object
```
New-PSSession -ComputerName (Get-Content Servers.txt | Select-Object -Skip 1)
```

### Example 7: Rename files and select several to review
```
Get-ChildItem *.txt -ReadOnly |
    Rename-Item -NewName {$_.BaseName + "-ro.txt"} -PassThru |
    Select-Object -First 5 -Wait
```

### Example 8: Demonstrate the intricacies of the -ExpandProperty parameter
```
# Create a custom object to use for the Select-Object example.
$object = [pscustomobject]@{Name="CustomObject";Expand=@(1,2,3,4,5)}
# Use the ExpandProperty parameter to Expand the property.
$object | Select-Object -ExpandProperty Expand -Property Name

1
2
3
4
5

# The output did not contain the Name property, but it was added successfully.
# Use Get-Member to confirm the Name property was added and populated.
$object | Select-Object -ExpandProperty Expand -Property Name | Get-Member

TypeName: System.Int32

Name        MemberType   Definition
----        ----------   ----------
CompareTo   Method       int CompareTo(System.Object value), int CompareTo(int value), int IComparable.CompareTo(System.Object obj)...
Equals      Method       bool Equals(System.Object obj), bool Equals(int obj), bool IEquatable[int].Equals(int other)
GetHashCode Method       int GetHashCode()
GetType     Method       type GetType()
GetTypeCode Method       System.TypeCode GetTypeCode(), System.TypeCode IConvertible.GetTypeCode()
ToBoolean   Method       bool IConvertible.ToBoolean(System.IFormatProvider provider)
ToByte      Method       byte IConvertible.ToByte(System.IFormatProvider provider)
ToChar      Method       char IConvertible.ToChar(System.IFormatProvider provider)
ToDateTime  Method       datetime IConvertible.ToDateTime(System.IFormatProvider provider)
ToDecimal   Method       decimal IConvertible.ToDecimal(System.IFormatProvider provider)
ToDouble    Method       double IConvertible.ToDouble(System.IFormatProvider provider)
ToInt16     Method       int16 IConvertible.ToInt16(System.IFormatProvider provider)
ToInt32     Method       int IConvertible.ToInt32(System.IFormatProvider provider)
ToInt64     Method       long IConvertible.ToInt64(System.IFormatProvider provider)
ToSByte     Method       sbyte IConvertible.ToSByte(System.IFormatProvider provider)
ToSingle    Method       float IConvertible.ToSingle(System.IFormatProvider provider)
ToString    Method       string ToString(), string ToString(string format), string ToString(System.IFormatProvider provider)...
ToType      Method       System.Object IConvertible.ToType(type conversionType, System.IFormatProvider provider)
ToUInt16    Method       uint16 IConvertible.ToUInt16(System.IFormatProvider provider)
ToUInt32    Method       uint32 IConvertible.ToUInt32(System.IFormatProvider provider)
ToUInt64    Method       uint64 IConvertible.ToUInt64(System.IFormatProvider provider)
Name        NoteProperty string Name=CustomObject
```

### Example 9: Create custom properties on objects
```
$customObject = 1 | Select-Object -Property MyCustomProperty
$customObject.MyCustomProperty = "New Custom Property"
$customObject

MyCustomProperty
----------------
New Custom Property
```

### Example 10: Create calculated properties for each InputObject
```
# Create a calculated property called $_.StartTime.DayOfWeek
Get-Process | Select-Object -Property ProcessName,{$_.StartTime.DayOfWeek}

ProcessName  $_.StartTime.DayOfWeek
----         ----------------------
alg                       Wednesday
ati2evxx                  Wednesday
ati2evxx                   Thursday
...

# Add a custom property to calculate the size in KiloBytes of each FileInfo object you pass in.
# Use the pipeline variable to divide each file's length by 1 KiloBytes
$size = @{label="Size(KB)";expression={$_.length/1KB}}
# Create an additional calculated property with the number of Days since the file was last accessed.
# You can also shorten the key names to be 'l', and 'e', or use Name instead of Label.
$days = @{l="Days";e={((Get-Date) - $_.LastAccessTime).Days}}
# You can also shorten the name of your label key to 'l' and your expression key to 'e'.
Get-ChildItem $PSHOME -File | Select-Object Name, $size, $days

Name                        Size(KB)        Days
----                        --------        ----
Certificate.format.ps1xml   12.5244140625   223
Diagnostics.Format.ps1xml   4.955078125     223
DotNetTypes.format.ps1xml   134.9833984375  223
```

## PARAMETERS

### -ExcludeProperty
Specifies the properties that this cmdlet excludes from the operation.
Wildcards are permitted.

Beginning in PowerShell 6, it is no longer required to include the Property parameter for ExcludeProperty to work.

```yaml
Type: System.String[]
Parameter Sets: DefaultParameter, SkipLastParameter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpandProperty
Specifies a property to select, and indicates that an attempt should be made to expand that property.

- If the specified property is an array, each value of the array is included in the output.
- If the specified property is an object, the objects properties are expanded for every InputObject In either case, the Type of objects output will match the Type of the expanded property.

If the Property parameter is specified, \`Select-Object\` will attempt to add each selected property as a NoteProperty to every outputted object.

\> \[!WARNING\] \> If you receive the error: Select : Property cannot be processed because property \`\<PropertyName\>\` \> already exists, consider the following.
\> Note that when using \`-ExpandProperty\`, \`Select-Object\` can not replace an existing property.
\> This means: \> \> - If the expanded object has a property of the same name, an error will occur.
\> - If the Selected object has a property of the same name as an Expanded objects property, an \>   error will occur.

```yaml
Type: System.String
Parameter Sets: DefaultParameter, SkipLastParameter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -First
Specifies the number of objects to select from the beginning of an array of input objects.

```yaml
Type: System.Int32
Parameter Sets: DefaultParameter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Index
Selects objects from an array based on their index values.
Enter the indexes in a comma-separated list.
Indexes in an array begin with 0, where 0 represents the first value and (n-1) represents the last value.

```yaml
Type: System.Int32[]
Parameter Sets: IndexParameter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Specifies objects to send to the cmdlet through the pipeline.
This parameter enables you to pipe objects to \`Select-Object\`.

When you pass objects to the InputObject parameter, instead of using the pipeline, \`Select-Object\` treats the InputObject as a single object, even if the value is a collection.
It is recommended that you use the pipeline when passing collections to \`Select-Object\`.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Last
Specifies the number of objects to select from the end of an array of input objects.

```yaml
Type: System.Int32
Parameter Sets: DefaultParameter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Specifies the properties to select.
These properties are added as NoteProperty members to the output objects.
Wildcards are permitted.

The value of the Property parameter can be a new calculated property.
To create a calculated, property, use a hash table.

Valid keys are:

- Name (or Label) - \`\<string\>\`
- Expression - \`\<string\>\` or \`\<script block\>\`

For more information, see about_Calculated_Properties (../Microsoft.PowerShell.Core/About/about_Calculated_Properties.md).

```yaml
Type: System.Object[]
Parameter Sets: DefaultParameter, SkipLastParameter
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Skips (does not select) the specified number of items.
By default, the Skip parameter counts from the beginning of the array or list of objects, but if the command uses the Last parameter, it counts from the end of the list or array.

Unlike the Index parameter, which starts counting at 0, the Skip parameter begins at 1.

```yaml
Type: System.Int32
Parameter Sets: DefaultParameter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkipIndex
@{Text=}

```yaml
Type: System.Int32[]
Parameter Sets: SkipIndexParameter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkipLast
Skips (does not select) the specified number of items from the end of the list or array.
Works in the same way as using Skip together with Last parameter.

Unlike the Index parameter, which starts counting at 0, the SkipLast parameter begins at 1.

```yaml
Type: System.Int32
Parameter Sets: SkipLastParameter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Unique
Specifies that if a subset of the input objects has identical properties and values, only a single member of the subset will be selected.

This parameter is case-sensitive.
As a result, strings that differ only in character casing are considered to be unique.

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

### -Wait
Indicates that the cmdlet turns off optimization.
PowerShell runs commands in the order that they appear in the command pipeline and lets them generate all objects.
By default, if you include a \`Select-Object\` command with the First or Index parameters in a command pipeline, PowerShell stops the command that generates the objects as soon as the selected number of objects is generated.

This parameter was introduced in Windows PowerShell 3.0.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: DefaultParameter, IndexParameter
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

### System.Management.Automation.PSObject
You can pipe any object to \`Select-Object\`.

## OUTPUTS

### System.Management.Automation.PSObject
## NOTES
- You can also refer to the \`Select-Object\` cmdlet by its built-in alias, \`select\`. For more   information, see about_Aliases (../Microsoft.PowerShell.Core/About/about_Aliases.md).
- The optimization feature of \`Select-Object\` is available only for commands that write objects to   the pipeline as they are processed. It has no effect on commands that buffer processed objects and   write them as a collection. Writing objects immediately is a cmdlet design best practice. For more   information, see Write Single Records to the Pipeline in Strongly Encouraged Development Guidelines (/powershell/scripting/developer/windows-powershell).

## RELATED LINKS

[about_Calculated_Properties]()

[Group-Object]()

[Sort-Object]()

[Where-Object]()

