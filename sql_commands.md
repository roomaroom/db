Some of The Most Important SQL Commands
SELECT - extracts data from a database
UPDATE - updates data in a database
DELETE - deletes data from a database
INSERT INTO - inserts new data into a database
CREATE DATABASE - creates a new database
ALTER DATABASE - modifies a database
CREATE TABLE - creates a new table
ALTER TABLE - modifies a table
DROP TABLE - deletes a table
CREATE INDEX - creates an index (search key)
DROP INDEX - deletes an index

##SQL SELECT
```
SELECT column_name,column_name
FROM table_name;

SELECT * FROM table_name;
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_columns

##SQL SELECT DISTINCT Syntax
```
SELECT DISTINCT column_name,column_name
FROM table_name;
```
##SQL WHERE Syntax
```
SELECT column_name,column_name
FROM table_name
WHERE column_name operator value;
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_where

##AND, OR Operator Example
```
SELECT * FROM Customers
WHERE Country='Germany'
AND City='Berlin';
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_where_and
```
SELECT * FROM Customers
WHERE City='Berlin'
OR City='München';
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_where_or
###Combining AND & OR
```
SELECT * FROM Customers
WHERE Country='Germany'
AND (City='Berlin' OR City='München');
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_where_and_or
##The SQL ORDER BY Keyword
```
SELECT column_name, column_name
FROM table_name
ORDER BY column_name ASC|DESC, column_name ASC|DESC;
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_orderby_desc
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_orderby3
##SQL INSERT INTO Syntax
The first form does not specify the column names where the data will be inserted, only their values:
```
INSERT INTO table_name
VALUES (value1,value2,value3,...);
The second form specifies both the column names and the values to be inserted:
```
```
INSERT INTO table_name (column1,column2,column3,...)
VALUES (value1,value2,value3,...);
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_insert_colname
http://www.w3schools.com/sql/trysql.asp?filename=trysql_insert_cols
##SQL UPDATE Syntax
```
UPDATE table_name
SET column1=value1,column2=value2,...
WHERE some_column=some_value;
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_update
##SQL DELETE Syntax
```
DELETE FROM table_name
WHERE some_column=some_value;
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_delete
##SQL LIKE Syntax
```
SELECT column_name(s)
FROM table_name
WHERE column_name LIKE pattern;
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_like
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_like_ending

##SQL CREATE INDEX
Indexes allow the database application to find data fast; without reading the whole table.
```
CREATE INDEX index_name
ON table_name (column_name)
```