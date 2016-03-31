##SQL JOIN
An SQL JOIN clause is used to combine rows from two or more tables, based on a common field between them.
The most common type of join is: SQL INNER JOIN (simple join). An SQL INNER JOIN returns all rows from multiple tables where the join condition is met.
The INNER JOIN keyword selects all rows from both tables as long as there is a match between the columns in both tables.
```
SELECT column_name(s)
FROM table1
JOIN table2
ON table1.column_name=table2.column_name;
```
![image] (http://www.w3schools.com/sql/img_innerjoin.gif)
```
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate
FROM Orders
INNER JOIN Customers
ON Orders.CustomerID=Customers.CustomerID;
```
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_join
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_join_inner
##Different SQL JOINs
Before we continue with examples, we will list the types of the different SQL JOINs you can use:

INNER JOIN: Returns all rows when there is at least one match in BOTH tables
LEFT JOIN: Return all rows from the left table, and the matched rows from the right table
RIGHT JOIN: Return all rows from the right table, and the matched rows from the left table
FULL JOIN: Return all rows when there is a match in ONE of the tables

##SQL LEFT JOIN Keyword
```
SELECT column_name(s)
FROM table1
LEFT JOIN table2
ON table1.column_name=table2.column_name;
```
![iamge] (http://www.w3schools.com/sql/img_leftjoin.gif)
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_join_left

##SQL RIGHT JOIN
```
SELECT column_name(s)
FROM table1
RIGHT JOIN table2
ON table1.column_name=table2.column_name;
```
![image](http://www.w3schools.com/sql/img_rightjoin.gif)
http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_join_right&ss=-1

##SQL FULL OUTER JOIN
```
SELECT column_name(s)
FROM table1
FULL OUTER JOIN table2
ON table1.column_name=table2.column_name;
```
![image](http://www.w3schools.com/sql/img_fulljoin.gif)
http://www.w3schools.com/sql/sql_join_full.asp