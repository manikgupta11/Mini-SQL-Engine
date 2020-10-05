# Mini-SQL-Engine

Python implementation of a mini SQL engine which runs a subset of SQL Queries using command line interface


List of queries that can be executed:
  ```

1. Select all records from 1 or multiple tables 
      Format: SELECT * FROM table_name

2. Aggragate functions (Sum, average, max, min) 
      Format: SELECT max(col1) FROM table_name

3. Project columns 
      Format: SELECT col1,col2 FROM table_name

4. Project with distinct from one table
      Format: SELECT distict(col1) FROM table_name

5. Select with "WHERE" condition( Relational operators "<, >, <=, >=, =" are handled )
      Format: SELECT * FROM table_name WHERE <condition>

6. Select with multiple "WHERE" conditions joined by AND/OR operator
      Format: SELECT * FROM table_name WHERE <condition-1> AND <condition-2>

7. Sort based on order specified in "ORDER BY" clause
      Format: SELECT * FROM table_1 ORDER BY col1,col2
      
8. Join 2 tables with/without "WHERE" condition
      Format: SELECT * FROM table_1,table_2 [WHERE <condition>]   

  ```
  


Data Format:

	1. .csv file for tables. File name table1.csv, table name is "table1" 

	2. metadata.txt file: having the structure for each table

	    eg. <begin_table> 
		<table_name> 
		<attribute1> 
		.... 
 
		<attributeN> 
		<end_table>  
