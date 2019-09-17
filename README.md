# ETL_AdventureWorks2016
project involves a retail company that sells a variety of products to people and to businesses across a variety of sales channels.
The Retail Company would like to: Create a data warehouse (DW) from its various systems of record (SORs) 
Create BI applications that enable analysis of business performance

# Problem Statement 

Extracting data from Source database and loading to target database

-Source database: 
<ul>
<li>
AdventureWorks2016_us - sql server 
</li>
<li>
AdventureWorks2016_eu - mysql  
</li>
<li>
AdventureWorks2016_au - postgresql  
</li>
<li>
AdventureWorks2016_ca - oracle 
</li>
</ul>
-	Target database: 
<ul>
<li>
AdventureWorksDW_neu: SQL Server for SSIS Target
</li></ul>

# Instructions

- Load all the source files into the databases
- Install ODBC driver for MySQL, PostgreSQL and Oracle (For SQL Server, you can use the OLE DB Source and Destination)
- Connect the source files using the ODBC Data sources
- Load the source data files to all the inputand output data components
- Change the path of all the flat files

Document on adding databases on ODBC drivers can be found [here](https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/ODBC_Connection.pdf)




# Source Files

<img width="540" alt="sources" src="https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/pictures/sources.jpeg">

# Target Tables

<img width="356" alt="target" src="https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/pictures/target.jpeg">

# Master Job to load the data warehouse at one click
<img width="895" alt="masterjob" src="https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/pictures/Master_Job.jpeg">

# Snapshots of few SSIS jobs

- DimEmployee
<img width="582" alt="dimemployee" src="https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/pictures/Dim_Employee.jpeg">

- SCD type 2 in DimEmployee

<img width="199" alt="scd2dimemployee" src="https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/pictures/SCD_Dim_Employee.jpeg">

- DimStore

![DimStore](https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/pictures/Dim_Store.jpeg)

- DimCustomer

![DimCustomer](https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/pictures/Dim_Customer.jpeg)

- FactInternetSales

![FactInternetSales](https://github.com/madhujagosavi/ETL_AdventureWorks2016/blob/master/pictures/Fact_Internet_Sales.jpeg)
