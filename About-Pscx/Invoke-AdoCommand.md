---
external help file: Pscx.dll-Help.xml
Module Name:
online version:
schema: 2.0.0
---

# Invoke-AdoCommand

## SYNOPSIS
PSCX Cmdlet: Execute a SQL query against an ADO.NET datasource.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Invoke-AdoCommand [-ProviderName] <String> [-Connection] <DbConnection> [-CommandText] <String> [-AsDataSet]
 [-AsPSObject] [-CommandType <CommandType>] [-NonQuery] [[-CommandParameters] <Hashtable>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_2
```
Invoke-AdoCommand [-ProviderName] <String> [-ConnectionProperties] <Hashtable> [-CommandText] <String>
 [-AsDataSet] [-AsPSObject] [-CommandType <CommandType>] [-NonQuery] [[-CommandParameters] <Hashtable>]
 [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_3
```
Invoke-AdoCommand [-ProviderName] <String> [-ConnectionString] <String> [-CommandText] <String> [-AsDataSet]
 [-AsPSObject] [-CommandType <CommandType>] [-NonQuery] [[-CommandParameters] <Hashtable>] [<CommonParameters>]
```

### UNNAMED_PARAMETER_SET_4
```
Invoke-AdoCommand [-ProviderName] <String> [-CommandText] <String> [-AsDataSet] [-AsPSObject]
 [-CommandType <CommandType>] [-Database <String>] [-NonQuery] [-Password <String>] [-Server <String>]
 [-UserName <String>] [[-CommandParameters] <Hashtable>] [<CommonParameters>]
```

## DESCRIPTION
Execute a SQL query against an ADO.NET datasource.

## EXAMPLES

### EXAMPLE 1
PS C:\\\>

```
$connection = Get-AdoProvider oracle | Get-AdoConnection -server orcl02 -username scott -password -tiger
          invoke-adocommand -connection $connection -commandtext "select * from foo"
```

This example fetches the oracle client provider and pipes it to Get-AdoConnection.
Using this technique
          means you don't have to know the specifics of any given database's connection string properties.

### EXAMPLE 2
PS C:\\\>

```
$conn = 'Data Source=.\SQLEXPRESS;Initial Catalog=pubs;Integrated Security=SSPI'
              $ds = Invoke-AdoCommand -ProviderName SqlClient -ConnectionString $conn -CommandText 'Select * from Authors' -AsDataSet
              $ds.Tables
              
              au_id    : 172-32-1176
              au_lname : White
              au_fname : Johnson
              ...
```

This example queries the pubs database for all authors on the current machine's SQLEXPRESS database instance.

## PARAMETERS

### -ProviderName
The name of the desired .NET data provider.
Typical values are System.Data.SqlClient, System.Data.OleDb,
                System.Data.Odbc and System.Data.OracleClient.
Accepts pipeline input from Get-AdoProvider command.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Connection
The connection object used in lieu of a connection string. 
This object is created using the 
                Get-AdoConnection cmdlet.

```yaml
Type: DbConnection
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectionProperties
Accepts a hashtable of one or more common connection properties such as Server, User, Password and Database.

```yaml
Type: Hashtable
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectionString
The connecion string required to connect to the database. 
For help with connection strings see
              the following link - http://msdn.microsoft.com/en-us/library/ms254500.aspx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommandText
The Transact-SQL statement, table name or stored procedure to execute at the data source.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: N/A
Accept pipeline input: False
Accept wildcard characters: False
```

### -AsDataSet
If specified returns the result as an ADO.NET DataSet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AsPSObject
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommandType
Specifies the type of command. 
Valid values are StoredProcedure, TableDirect and Text. 
The default value is Text.

```yaml
Type: CommandType
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: Text
Accept pipeline input: False
Accept wildcard characters: False
```

### -Database
The name of the current database or the database to be used after a connection is opened.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NonQuery
Executes a command returning the number of rows affected. 
If specified then -AsDataSet is ignored.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Password
The password to use when connecting to the target server.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Server
The name of the host or named instance (with MSSQL) to connect to.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserName
The username to use when connecting to the target server.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommandParameters
The parameters of the Transact-SQL statement or stored procedure.
The default is an empty collection.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: Empty parameter collection.
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
* 
            The typical problem encountered when using the ConnectionString property is getting the connection string right.
            See the following link for help with connection strings - http://msdn.microsoft.com/en-us/library/ms254500.aspx.
            For this reason, this Cmdlet uses the built-in .NET data factory classes when using the ConnectionProperties
            parameter or the individual connection property parameters. Thankfully, you don't need to know the specifics
            of a support database's connection string properties. The Server, Username, Password and Database properties are
            automatically translated to the target database's format.

## RELATED LINKS
