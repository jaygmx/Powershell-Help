---
external help file: ImportExcel-help.xml
Module Name: ImportExcel
online version:
schema: 2.0.0
---

# Send-SQLDataToExcel

## SYNOPSIS
Inserts a DataTable - returned by a SQL query - into an ExcelSheet

## SYNTAX

### none (Default)
```
Send-SQLDataToExcel [-QueryTimeout <Int32>] [-Force] [-Path <String>] [-ExcelPackage <ExcelPackage>]
 [-Calculate] [-Show] [-WorksheetName <String>] [-Password <String>] [-ClearSheet] [-Append] [-Title <String>]
 [-TitleFillPattern <ExcelFillStyle>] [-TitleBold] [-TitleSize <Int32>] [-TitleBackgroundColor <Object>]
 [-IncludePivotTable] [-PivotTableName <String>] [-PivotRows <String[]>] [-PivotColumns <String[]>]
 [-PivotData <Object>] [-PivotFilter <String[]>] [-PivotDataToColumn] [-PivotTableDefinition <Hashtable>]
 [-IncludePivotChart] [-PivotChartType <eChartType>] [-NoLegend] [-ShowCategory] [-ShowPercent] [-AutoSize]
 [-MaxAutoSizeRows <Object>] [-NoClobber] [-FreezeTopRow] [-FreezeFirstColumn] [-FreezeTopRowFirstColumn]
 [-FreezePane <Int32[]>] [-AutoFilter] [-BoldTopRow] [-NoHeader] [-RangeName <String>] [-TableName <Object>]
 [-TableStyle <TableStyles>] [-Barchart] [-PieChart] [-LineChart] [-ColumnChart]
 [-ExcelChartDefinition <Object[]>] [-HideSheet <String[]>] [-UnHideSheet <String[]>] [-MoveToStart]
 [-MoveToEnd] [-MoveBefore <Object>] [-MoveAfter <Object>] [-KillExcel] [-AutoNameRange] [-StartRow <Int32>]
 [-StartColumn <Int32>] [-PassThru] [-Numberformat <String>] [-ExcludeProperty <String[]>]
 [-NoAliasOrScriptPropeties] [-DisplayPropertySet] [-NoNumberConversion <String[]>]
 [-ConditionalFormat <Object[]>] [-ConditionalText <Object[]>] [-Style <Object[]>] [-CellStyleSB <ScriptBlock>]
 [-Activate] [-Now] [-ReturnRange] [-PivotTotals <String>] [-NoTotalsInPivot] [-ReZip] [<CommonParameters>]
```

### ODBCConnection
```
Send-SQLDataToExcel -Connection <Object> -SQL <String> [-QueryTimeout <Int32>] [-Force] [-Path <String>]
 [-ExcelPackage <ExcelPackage>] [-Calculate] [-Show] [-WorksheetName <String>] [-Password <String>]
 [-ClearSheet] [-Append] [-Title <String>] [-TitleFillPattern <ExcelFillStyle>] [-TitleBold]
 [-TitleSize <Int32>] [-TitleBackgroundColor <Object>] [-IncludePivotTable] [-PivotTableName <String>]
 [-PivotRows <String[]>] [-PivotColumns <String[]>] [-PivotData <Object>] [-PivotFilter <String[]>]
 [-PivotDataToColumn] [-PivotTableDefinition <Hashtable>] [-IncludePivotChart] [-PivotChartType <eChartType>]
 [-NoLegend] [-ShowCategory] [-ShowPercent] [-AutoSize] [-MaxAutoSizeRows <Object>] [-NoClobber]
 [-FreezeTopRow] [-FreezeFirstColumn] [-FreezeTopRowFirstColumn] [-FreezePane <Int32[]>] [-AutoFilter]
 [-BoldTopRow] [-NoHeader] [-RangeName <String>] [-TableName <Object>] [-TableStyle <TableStyles>] [-Barchart]
 [-PieChart] [-LineChart] [-ColumnChart] [-ExcelChartDefinition <Object[]>] [-HideSheet <String[]>]
 [-UnHideSheet <String[]>] [-MoveToStart] [-MoveToEnd] [-MoveBefore <Object>] [-MoveAfter <Object>]
 [-KillExcel] [-AutoNameRange] [-StartRow <Int32>] [-StartColumn <Int32>] [-PassThru] [-Numberformat <String>]
 [-ExcludeProperty <String[]>] [-NoAliasOrScriptPropeties] [-DisplayPropertySet]
 [-NoNumberConversion <String[]>] [-ConditionalFormat <Object[]>] [-ConditionalText <Object[]>]
 [-Style <Object[]>] [-CellStyleSB <ScriptBlock>] [-Activate] [-Now] [-ReturnRange] [-PivotTotals <String>]
 [-NoTotalsInPivot] [-ReZip] [<CommonParameters>]
```

### SQLConnection
```
Send-SQLDataToExcel -Connection <Object> [-MsSqlServer] [-DataBase <String>] -SQL <String>
 [-QueryTimeout <Int32>] [-Force] [-Path <String>] [-ExcelPackage <ExcelPackage>] [-Calculate] [-Show]
 [-WorksheetName <String>] [-Password <String>] [-ClearSheet] [-Append] [-Title <String>]
 [-TitleFillPattern <ExcelFillStyle>] [-TitleBold] [-TitleSize <Int32>] [-TitleBackgroundColor <Object>]
 [-IncludePivotTable] [-PivotTableName <String>] [-PivotRows <String[]>] [-PivotColumns <String[]>]
 [-PivotData <Object>] [-PivotFilter <String[]>] [-PivotDataToColumn] [-PivotTableDefinition <Hashtable>]
 [-IncludePivotChart] [-PivotChartType <eChartType>] [-NoLegend] [-ShowCategory] [-ShowPercent] [-AutoSize]
 [-MaxAutoSizeRows <Object>] [-NoClobber] [-FreezeTopRow] [-FreezeFirstColumn] [-FreezeTopRowFirstColumn]
 [-FreezePane <Int32[]>] [-AutoFilter] [-BoldTopRow] [-NoHeader] [-RangeName <String>] [-TableName <Object>]
 [-TableStyle <TableStyles>] [-Barchart] [-PieChart] [-LineChart] [-ColumnChart]
 [-ExcelChartDefinition <Object[]>] [-HideSheet <String[]>] [-UnHideSheet <String[]>] [-MoveToStart]
 [-MoveToEnd] [-MoveBefore <Object>] [-MoveAfter <Object>] [-KillExcel] [-AutoNameRange] [-StartRow <Int32>]
 [-StartColumn <Int32>] [-PassThru] [-Numberformat <String>] [-ExcludeProperty <String[]>]
 [-NoAliasOrScriptPropeties] [-DisplayPropertySet] [-NoNumberConversion <String[]>]
 [-ConditionalFormat <Object[]>] [-ConditionalText <Object[]>] [-Style <Object[]>] [-CellStyleSB <ScriptBlock>]
 [-Activate] [-Now] [-ReturnRange] [-PivotTotals <String>] [-NoTotalsInPivot] [-ReZip] [<CommonParameters>]
```

### ExistingSession
```
Send-SQLDataToExcel -Session <Object> -SQL <String> [-QueryTimeout <Int32>] [-Force] [-Path <String>]
 [-ExcelPackage <ExcelPackage>] [-Calculate] [-Show] [-WorksheetName <String>] [-Password <String>]
 [-ClearSheet] [-Append] [-Title <String>] [-TitleFillPattern <ExcelFillStyle>] [-TitleBold]
 [-TitleSize <Int32>] [-TitleBackgroundColor <Object>] [-IncludePivotTable] [-PivotTableName <String>]
 [-PivotRows <String[]>] [-PivotColumns <String[]>] [-PivotData <Object>] [-PivotFilter <String[]>]
 [-PivotDataToColumn] [-PivotTableDefinition <Hashtable>] [-IncludePivotChart] [-PivotChartType <eChartType>]
 [-NoLegend] [-ShowCategory] [-ShowPercent] [-AutoSize] [-MaxAutoSizeRows <Object>] [-NoClobber]
 [-FreezeTopRow] [-FreezeFirstColumn] [-FreezeTopRowFirstColumn] [-FreezePane <Int32[]>] [-AutoFilter]
 [-BoldTopRow] [-NoHeader] [-RangeName <String>] [-TableName <Object>] [-TableStyle <TableStyles>] [-Barchart]
 [-PieChart] [-LineChart] [-ColumnChart] [-ExcelChartDefinition <Object[]>] [-HideSheet <String[]>]
 [-UnHideSheet <String[]>] [-MoveToStart] [-MoveToEnd] [-MoveBefore <Object>] [-MoveAfter <Object>]
 [-KillExcel] [-AutoNameRange] [-StartRow <Int32>] [-StartColumn <Int32>] [-PassThru] [-Numberformat <String>]
 [-ExcludeProperty <String[]>] [-NoAliasOrScriptPropeties] [-DisplayPropertySet]
 [-NoNumberConversion <String[]>] [-ConditionalFormat <Object[]>] [-ConditionalText <Object[]>]
 [-Style <Object[]>] [-CellStyleSB <ScriptBlock>] [-Activate] [-Now] [-ReturnRange] [-PivotTotals <String>]
 [-NoTotalsInPivot] [-ReZip] [<CommonParameters>]
```

### Pre-FetchedData
```
Send-SQLDataToExcel [-QueryTimeout <Int32>] -DataTable <DataTable> [-Force] [-Path <String>]
 [-ExcelPackage <ExcelPackage>] [-Calculate] [-Show] [-WorksheetName <String>] [-Password <String>]
 [-ClearSheet] [-Append] [-Title <String>] [-TitleFillPattern <ExcelFillStyle>] [-TitleBold]
 [-TitleSize <Int32>] [-TitleBackgroundColor <Object>] [-IncludePivotTable] [-PivotTableName <String>]
 [-PivotRows <String[]>] [-PivotColumns <String[]>] [-PivotData <Object>] [-PivotFilter <String[]>]
 [-PivotDataToColumn] [-PivotTableDefinition <Hashtable>] [-IncludePivotChart] [-PivotChartType <eChartType>]
 [-NoLegend] [-ShowCategory] [-ShowPercent] [-AutoSize] [-MaxAutoSizeRows <Object>] [-NoClobber]
 [-FreezeTopRow] [-FreezeFirstColumn] [-FreezeTopRowFirstColumn] [-FreezePane <Int32[]>] [-AutoFilter]
 [-BoldTopRow] [-NoHeader] [-RangeName <String>] [-TableName <Object>] [-TableStyle <TableStyles>] [-Barchart]
 [-PieChart] [-LineChart] [-ColumnChart] [-ExcelChartDefinition <Object[]>] [-HideSheet <String[]>]
 [-UnHideSheet <String[]>] [-MoveToStart] [-MoveToEnd] [-MoveBefore <Object>] [-MoveAfter <Object>]
 [-KillExcel] [-AutoNameRange] [-StartRow <Int32>] [-StartColumn <Int32>] [-PassThru] [-Numberformat <String>]
 [-ExcludeProperty <String[]>] [-NoAliasOrScriptPropeties] [-DisplayPropertySet]
 [-NoNumberConversion <String[]>] [-ConditionalFormat <Object[]>] [-ConditionalText <Object[]>]
 [-Style <Object[]>] [-CellStyleSB <ScriptBlock>] [-Activate] [-Now] [-ReturnRange] [-PivotTotals <String>]
 [-NoTotalsInPivot] [-ReZip] [<CommonParameters>]
```

## DESCRIPTION
This command takes a SQL statement and run it against a database connection; for the connection it accepts either

* an object representing a session with a SQL server or ODBC database, or
* a connection string to make a session (if -MSSQLServer is specified it uses the SQL Native client,

and -Connection can be a server name instead of a detailed connection string.
Without this switch it uses ODBC)

The command takes all the parameters of Export-Excel, except for -InputObject (alias TargetData); after fetching the data it calls Export-Excel with the data as the value of InputParameter and whichever of Export-Excel's parameters it was passed; for details of these parameters see the help for Export-Excel.

## EXAMPLES

### EXAMPLE 1
```
PS\> Send-SQLDataToExcel -MsSQLserver -Connection localhost -SQL  "select name,type,type_desc from [master].[sys].[all_objects]" -Path .\temp.xlsx -WorkSheetname master -AutoSize -FreezeTopRow -AutoFilter -BoldTopRow
```

Connects to the local SQL server and selects 3 columns from \[Sys\].\[all_objects\] and exports then to a sheet named master with some basic header management

### EXAMPLE 2
```
PS\> $dbPath = 'C:\Users\James\Documents\Database1.accdb'
PS\> $Connection = "Driver={Microsoft Access Driver (*.mdb, *.accdb)};Dbq=$dbPath;"
PS\> $SQL="SELECT top 25 Name,Length  From TestData ORDER BY Length DESC"
PS\> Send-SQLDataToExcel -Connection  $connection -SQL $sql -path .\demo1.xlsx -WorkSheetname "Sizes" -AutoSize
```

This creates an  ODBC connection string to read from an Access file and a SQL Statement to extracts data from it, and sends the resulting data to a new worksheet

### EXAMPLE 3
```
PS\> $dbPath = 'C:\users\James\Documents\f1Results.xlsx'

PS\> $Connection = "Driver={Microsoft Excel Driver (*.xls, *.xlsx, *.xlsm, *.xlsb)};Dbq=$dbPath;"
PS\> $SQL="SELECT top 25 DriverName, Count(RaceDate) as Races, Count(Win) as Wins, Count(Pole) as Poles, Count(FastestLap) as Fastlaps " +
           " FROM Results  GROUP BY DriverName ORDER BY (count(win)) DESC"

PS\>Send-SQLDataToExcel -Connection  $connection -SQL $sql -path .\demo2.xlsx -WorkSheetname "Winners" -AutoSize -AutoNameRange -ConditionalFormat @{DataBarColor="Blue"; Range="Wins"}
```

Similar to the previous example, this creates a connection string, this time for an Excel file, and runs a SQL statement to get a list of motor-racing results, outputting the resulting data to a new spreadsheet.
The spreadsheet is formatted and a data bar added to show make the drivers' wins clearer.
(The F1 results database is available from https://1drv.ms/x/s!AhfYu7-CJv4ehNdZWxJE9LMAX_N5sg )

### EXAMPLE 4
```
PS\> $dbPath = 'C:\users\James\Documents\f1Results.xlsx'

PS\> $SQL = "SELECT top 25 DriverName, Count(RaceDate) as Races, Count(Win) as Wins, Count(Pole) as Poles, Count(FastestLap) as Fastlaps " +
             " FROM Results GROUP BY DriverName ORDER BY (count(win)) DESC"
PS\> $null = Get-SQL -Session F1 -excel -Connection $dbPath -sql $sql -OutputVariable Table

PS\> Send-SQLDataToExcel -DataTable $Table -Path ".\demo3.xlsx" -WorkSheetname Gpwinners -autosize  -TableName winners -TableStyle Light6 -show
```

This uses Get-SQL (at least V1.1 - download from the PowerShell gallery with Install-Module -Name GetSQL - (note the function is Get-SQL the module is GetSQL without the "-" )

Get-SQL simplifies making database connections and building /submitting SQL statements.
Here Get-SQL uses the same SQL statement as before; -OutputVariable leaves a System.Data.DataTable object in $table  and Send-SQLDataToExcel puts $table into the worksheet and sets it as an Excel table.
The command is equivalent to running

PS\>  Export-Excel -inputObject $Table -Path ".\demo3.xlsx" -WorkSheetname Gpwinners -autosize  -TableName winners -TableStyle Light6 -show

This is quicker than using PS\> Get-SQL \<parameters\> | export-excel -ExcludeProperty rowerror,rowstate,table,itemarray,haserrors \<parameters\>

(the F1 results database is available from https://1drv.ms/x/s!AhfYu7-CJv4ehNdZWxJE9LMAX_N5sg )

### EXAMPLE 5
```
PS\>$SQL = "SELECT top 25 DriverName,  Count(Win) as Wins FROM Results GROUP BY DriverName ORDER BY (count(win)) DESC"
PS\> Send-SQLDataToExcel -Session $DbSessions\["f1"\] -SQL $sql -Path  ".\demo3.xlsx" -WorkSheetname Gpwinners  -ClearSheet -autosize -ColumnChart
```

Like the previous example, this uses Get-SQL (download from the gallery with Install-Module -Name GetSQL).
It uses the database session which Get-SQL created, rather than an ODBC connection string.
The Session parameter can either be a object (as shown here), or the name used by Get-SQL ("F1" in this case).

Here the data is presented as a quick chart.

### EXAMPLE 6
```
Send-SQLDataToExcel -path .\demo4.xlsx -WorkSheetname "LR" -Connection "DSN=LR" -sql "SELECT name AS CollectionName FROM AgLibraryCollection Collection ORDER BY CollectionName"
```

This example uses an Existing ODBC datasource name "LR" which maps to an adobe lightroom database and gets a list of collection names into a worksheet

## PARAMETERS

### -Connection
A database connection string to be used to create a database session; either

* A Data source name written in the form DSN=ODBC_Data_Source_Name, or
* A full ODBC or SQL Native Client Connection string, or
* The name of a SQL server.

```yaml
Type: System.Object
Parameter Sets: ODBCConnection, SQLConnection
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Session
An active ODBC Connection or SQL connection object representing a session with a database which will be queried to get the data .

```yaml
Type: System.Object
Parameter Sets: ExistingSession
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DataBase
Switches to a specific database on a SQL server.

```yaml
Type: System.String
Parameter Sets: SQLConnection
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SQL
The SQL query to run against the session which was passed in -Session or set up from -Connection.

```yaml
Type: System.String
Parameter Sets: ODBCConnection, SQLConnection, ExistingSession
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -QueryTimeout
Override the default query time of 30 seconds.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -DataTable
A System.Data.DataTable object containing the data to be inserted into the spreadsheet without running a query.
This remains supported to avoid breaking older scripts, but if you have a DataTable object you can pass the it into Export-Excel using -InputObject.

```yaml
Type: System.Data.DataTable
Parameter Sets: Pre-FetchedData
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
If specified Export-Excel will be called with parameters specified, even if there is no data to send

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

### -Activate
{{ Fill Activate Description }}

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

### -Append
{{ Fill Append Description }}

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

### -AutoFilter
{{ Fill AutoFilter Description }}

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

### -AutoNameRange
{{ Fill AutoNameRange Description }}

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

### -AutoSize
{{ Fill AutoSize Description }}

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

### -Barchart
{{ Fill Barchart Description }}

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

### -BoldTopRow
{{ Fill BoldTopRow Description }}

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

### -Calculate
{{ Fill Calculate Description }}

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

### -CellStyleSB
{{ Fill CellStyleSB Description }}

```yaml
Type: System.Management.Automation.ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClearSheet
{{ Fill ClearSheet Description }}

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

### -ColumnChart
{{ Fill ColumnChart Description }}

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

### -ConditionalFormat
{{ Fill ConditionalFormat Description }}

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

### -ConditionalText
{{ Fill ConditionalText Description }}

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

### -DisplayPropertySet
{{ Fill DisplayPropertySet Description }}

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

### -ExcelChartDefinition
{{ Fill ExcelChartDefinition Description }}

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

### -ExcelPackage
{{ Fill ExcelPackage Description }}

```yaml
Type: OfficeOpenXml.ExcelPackage
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExcludeProperty
{{ Fill ExcludeProperty Description }}

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

### -FreezeFirstColumn
{{ Fill FreezeFirstColumn Description }}

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

### -FreezePane
{{ Fill FreezePane Description }}

```yaml
Type: System.Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FreezeTopRow
{{ Fill FreezeTopRow Description }}

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

### -FreezeTopRowFirstColumn
{{ Fill FreezeTopRowFirstColumn Description }}

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

### -HideSheet
{{ Fill HideSheet Description }}

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

### -IncludePivotChart
{{ Fill IncludePivotChart Description }}

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

### -IncludePivotTable
{{ Fill IncludePivotTable Description }}

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

### -KillExcel
{{ Fill KillExcel Description }}

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

### -LineChart
{{ Fill LineChart Description }}

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

### -MaxAutoSizeRows
{{ Fill MaxAutoSizeRows Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MoveAfter
{{ Fill MoveAfter Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MoveBefore
{{ Fill MoveBefore Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MoveToEnd
{{ Fill MoveToEnd Description }}

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

### -MoveToStart
{{ Fill MoveToStart Description }}

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

### -MsSqlServer
Specifies the connection string is for SQL server, not ODBC.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: SQLConnection
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoAliasOrScriptPropeties
{{ Fill NoAliasOrScriptPropeties Description }}

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

### -NoClobber
{{ Fill NoClobber Description }}

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

### -NoHeader
{{ Fill NoHeader Description }}

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

### -NoLegend
{{ Fill NoLegend Description }}

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

### -NoNumberConversion
{{ Fill NoNumberConversion Description }}

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

### -NoTotalsInPivot
{{ Fill NoTotalsInPivot Description }}

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

### -Now
{{ Fill Now Description }}

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

### -Numberformat
{{ Fill Numberformat Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
{{ Fill PassThru Description }}

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

### -Password
{{ Fill Password Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
{{ Fill Path Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PieChart
{{ Fill PieChart Description }}

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

### -PivotChartType
{{ Fill PivotChartType Description }}

```yaml
Type: OfficeOpenXml.Drawing.Chart.eChartType
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PivotColumns
{{ Fill PivotColumns Description }}

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

### -PivotData
{{ Fill PivotData Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PivotDataToColumn
{{ Fill PivotDataToColumn Description }}

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

### -PivotFilter
{{ Fill PivotFilter Description }}

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

### -PivotRows
{{ Fill PivotRows Description }}

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

### -PivotTableDefinition
{{ Fill PivotTableDefinition Description }}

```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PivotTableName
{{ Fill PivotTableName Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PivotTotals
{{ Fill PivotTotals Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RangeName
{{ Fill RangeName Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReturnRange
{{ Fill ReturnRange Description }}

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

### -ReZip
{{ Fill ReZip Description }}

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

### -Show
{{ Fill Show Description }}

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

### -ShowCategory
{{ Fill ShowCategory Description }}

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

### -ShowPercent
{{ Fill ShowPercent Description }}

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

### -StartColumn
{{ Fill StartColumn Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartRow
{{ Fill StartRow Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Style
{{ Fill Style Description }}

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

### -TableName
{{ Fill TableName Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TableStyle
{{ Fill TableStyle Description }}

```yaml
Type: OfficeOpenXml.Table.TableStyles
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Title
{{ Fill Title Description }}

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleBackgroundColor
{{ Fill TitleBackgroundColor Description }}

```yaml
Type: System.Object
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleBold
{{ Fill TitleBold Description }}

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

### -TitleFillPattern
{{ Fill TitleFillPattern Description }}

```yaml
Type: OfficeOpenXml.Style.ExcelFillStyle
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleSize
{{ Fill TitleSize Description }}

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UnHideSheet
{{ Fill UnHideSheet Description }}

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

### -WorksheetName
{{ Fill WorksheetName Description }}

```yaml
Type: System.String
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

## OUTPUTS

## NOTES

## RELATED LINKS

[Export-Excel]()
