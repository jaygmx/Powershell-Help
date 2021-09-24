---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
Module Name: Microsoft.PowerShell.Utility
online version: https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/add-member?view=powershell-7.1&WT.mc_id=ps-gethelp
schema: 2.0.0
---

# Add-Member

## SYNOPSIS
Adds custom properties and methods to an instance of a PowerShell object.

## SYNTAX

### TypeNameSet (Default)
```
Add-Member -InputObject <PSObject> -TypeName <String> [-PassThru] [<CommonParameters>]
```

### NotePropertySingleMemberSet
```
Add-Member -InputObject <PSObject> [-TypeName <String>] [-Force] [-PassThru] [-NotePropertyName] <String>
 [-NotePropertyValue] <Object> [<CommonParameters>]
```

### MemberSet
```
Add-Member -InputObject <PSObject> [-MemberType] <PSMemberTypes> [-Name] <String> [[-Value] <Object>]
 [[-SecondValue] <Object>] [-TypeName <String>] [-Force] [-PassThru] [<CommonParameters>]
```

### NotePropertyMultiMemberSet
```
Add-Member -InputObject <PSObject> [-TypeName <String>] [-Force] [-PassThru]
 [-NotePropertyMembers] <IDictionary> [<CommonParameters>]
```

## DESCRIPTION
The \`Add-Member\` cmdlet lets you add members (properties and methods) to an instance of a PowerShell object.
For instance, you can add a NoteProperty member that contains a description of the object or a ScriptMethod member that runs a script to change the object.

To use \`Add-Member\`, pipe the object to \`Add-Member\`, or use the InputObject parameter to specify the object.

The MemberType parameter indicates the type of member that you want to add.
The Name parameter assigns a name to the new member, and the Value parameter sets the value of the member.

The properties and methods that you add are added only to the particular instance of the object that you specify.
\`Add-Member\` does not change the object type.
To create a new object type, use the \`Add-Type\` cmdlet.

You can also use the \`Export-Clixml\` cmdlet to save the instance of the object, including the additional members, in a file.
Then you can use the \`Import-Clixml\` cmdlet to re-create the instance of the object from the information that is stored in the exported file.

Beginning in Windows PowerShell 3.0, \`Add-Member\` has new features that make it easier to add note properties to objects.
You can use the NotePropertyName and NotePropertyValue parameters to define a note property or use the NotePropertyMembers parameter, which takes a hash table of note property names and values.

Also, beginning in Windows PowerShell 3.0, the PassThru parameter, which generates an output object, is needed less frequently.
\`Add-Member\` now adds the new members directly to the input object of more types.
For more information, see the PassThru parameter description.

## EXAMPLES

### Example 1: Add a note property to a PSObject
```
$A = Get-ChildItem c:\ps-test\test.txt
$A | Add-Member -NotePropertyName Status -NotePropertyValue Done
$A.Status

Done
```

### Example 2: Add an alias property to a PSObject
```
$A = Get-ChildItem C:\Temp\test.txt
$A | Add-Member -MemberType AliasProperty -Name Size -Value Length
$A.Size

2394
```

### Example 3: Add a StringUse note property to a string
```
$A = "A string"
$A = $A | Add-Member -NotePropertyMembers @{StringUse="Display"} -PassThru
$A.StringUse

Display
```

### Example 4: Add a script method to a FileInfo object
```
$A = Get-ChildItem C:\Temp\test.txt
$S = {[math]::Round(($this.Length / 1MB), 2)}
$A | Add-Member -MemberType ScriptMethod -Name "SizeInMB" -Value $S
$A.SizeInMB()

0.43
```

### Example 5: Copy all properties of an object to another
```
function Copy-Property ($From, $To)
{
    $properties = Get-Member -InputObject $From -MemberType Property
    foreach ($p in $properties)
    {
        $To | Add-Member -MemberType NoteProperty -Name $p.Name -Value $From.$($p.Name) -Force
    }
}
```

### Example 6: Create a custom object
```
$Asset = New-Object -TypeName PSObject
$d = [ordered]@{Name="Server30";System="Server Core";PSVersion="4.0"}
$Asset | Add-Member -NotePropertyMembers $d -TypeName Asset
$Asset | Get-Member

TypeName: Asset

Name        MemberType   Definition
----        ----------   ----------
Equals      Method       bool Equals(System.Object obj)
GetHashCode Method       int GetHashCode()
GetType     Method       type GetType()
ToString    Method       string ToString()
Name        NoteProperty System.String Name=Server30
PSVersion   NoteProperty System.String PSVersion=4.0
System      NoteProperty System.String System=Server Core
```

## PARAMETERS

### -Force
Indicates that this cmdlet adds a new member even the object has a custom member with the same name.
You cannot use the Force parameter to replace a standard member of a type.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: NotePropertySingleMemberSet, MemberSet, NotePropertyMultiMemberSet
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Specifies the object to which the new member is added.
Enter a variable that contains the objects, or type a command or expression that gets the objects.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MemberType
Specifies the type of the member to add.
This parameter is required.
The acceptable values for this parameter are:

- NoteProperty
- AliasProperty
- ScriptProperty
- CodeProperty
- ScriptMethod
- CodeMethod

For information about these values, see PSMemberTypes Enumeration (/dotnet/api/system.management.automation.psmembertypes)in the PowerShell SDK.

Not all objects have every type of member.
If you specify a member type that the object does not have, PowerShell returns an error.

```yaml
Type: System.Management.Automation.PSMemberTypes
Parameter Sets: MemberSet
Aliases: Type
Accepted values: AliasProperty, CodeProperty, Property, NoteProperty, ScriptProperty, Properties, PropertySet, Method, CodeMethod, ScriptMethod, Methods, ParameterizedProperty, MemberSet, Event, Dynamic, All

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the member that this cmdlet adds.

```yaml
Type: System.String
Parameter Sets: MemberSet
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NotePropertyMembers
Specifies a hash table or ordered dictionary of note property names and values.
Type a hash table or dictionary in which the keys are note property names and the values are note property values.

For more information about hash tables and ordered dictionaries in PowerShell, see about_Hash_Tables (../Microsoft.PowerShell.Core/About/about_Hash_Tables.md).

This parameter was introduced in Windows PowerShell 3.0.

```yaml
Type: System.Collections.IDictionary
Parameter Sets: NotePropertyMultiMemberSet
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NotePropertyName
Specifies the note property name.

Use this parameter with the NotePropertyValue parameter.
This parameter is optional.

This parameter was introduced in Windows PowerShell 3.0.

```yaml
Type: System.String
Parameter Sets: NotePropertySingleMemberSet
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NotePropertyValue
Specifies the note property value.

Use this parameter with the NotePropertyName parameter.
This parameter is optional.

This parameter was introduced in Windows PowerShell 3.0.

```yaml
Type: System.Object
Parameter Sets: NotePropertySingleMemberSet
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

For most objects, \`Add-Member\` adds the new members to the input object.
However, when the input object is a string, \`Add-Member\` cannot add the member to the input object.
For these objects, use the PassThru parameter to create an output object.

In Windows PowerShell 2.0, \`Add-Member\` added members only to the PSObject wrapper of objects, not to the object.
Use the PassThru parameter to create an output object for any object that has a PSObject wrapper.

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

### -SecondValue
Specifies optional additional information about AliasProperty , ScriptProperty , CodeProperty , or CodeMethod members.

If used when adding an AliasProperty , this parameter must be a data type.
A conversion to the specified data type is added to the value of the AliasProperty .

For example, if you add an AliasProperty that provides an alternate name for a string property, you can also specify a SecondValue parameter of System.Int32 to indicate that the value of that string property should be converted to an integer when accessed by using the corresponding AliasProperty .

You can use the SecondValue parameter to specify an additional ScriptBlock when adding a ScriptProperty member.
The first ScriptBlock , specified in the Value parameter, is used to get the value of a variable.
The second ScriptBlock , specified in the SecondValue parameter, is used to set the value of a variable.

```yaml
Type: System.Object
Parameter Sets: MemberSet
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TypeName
Specifies a name for the type.

When the type is a class in the System namespace or a type that has a type accelerator, you can enter the short name of the type.
Otherwise, the full type name is required.
This parameter is effective only when the InputObject is a PSObject .

This parameter was introduced in Windows PowerShell 3.0.

```yaml
Type: System.String
Parameter Sets: TypeNameSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: System.String
Parameter Sets: NotePropertySingleMemberSet, MemberSet, NotePropertyMultiMemberSet
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value
Specifies the initial value of the added member.
If you add an AliasProperty , CodeProperty , ScriptProperty or CodeMethod member, you can supply optional, additional information by using the SecondValue parameter.

```yaml
Type: System.Object
Parameter Sets: MemberSet
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Management.Automation.PSObject
You can pipe any object type to this cmdlet.

## OUTPUTS

### None or System.Object
When you use the PassThru parameter, this cmdlet returns the newly-extended object.
Otherwise, this cmdlet does not generate any output.

## NOTES
You can add members only to PSObject objects.
To determine whether an object is a PSObject object, use the \`-is\` operator.

For instance, to test an object stored in the \`$obj\` variable, type \`$obj -is \[PSObject\]\`.

The names of the MemberType , Name , Value , and SecondValue parameters are optional.
If you omit the parameter names, the unnamed parameter values must appear in this order: MemberType , Name , Value , and SecondValue .

If you include the parameter names, the parameters can appear in any order.

You can use the \`$this\` automatic variable in script blocks that define the values of new properties and methods.
The \`$this\` variable refers to the instance of the object to which the properties and methods are being added.
For more information about the \`$this\` variable, see about_Automatic_Variables (../Microsoft.PowerShell.Core/About/about_Automatic_Variables.md).

## RELATED LINKS

[Export-Clixml]()

[Get-Member]()

[Import-Clixml]()

[New-Object]()

[about_Automatic_Variables]()

