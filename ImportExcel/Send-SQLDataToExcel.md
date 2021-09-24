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

