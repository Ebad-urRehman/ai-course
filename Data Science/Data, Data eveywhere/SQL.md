Structured Query Language


Data go on forever, spread sheet is not the best option for very large datasets.
Database provides way, to organize, retrieve and analyze data.

Data bases
Postgre SQL
MySQL


Query : A request for data or information from a database. 

### Structure of Basic query : 
![[Pasted image 20241027161340.png]]E

Example : 
SELECT * FROM DATA.column_name
WHERE col_name = 'Value'


SELECT
ColumnA,
ColumnB,
ColumnC
FROM
Table where the data lives
WHERE
Condition 1
AND Condition 2
AND Condition 3

SELECT uses , to separate columns , while WHERE uses AND  to separate conditions

## Key takeaways

The SELECT, FROM, and WHERE clauses are the essential building blocks of SQL queries. Queries with multiple fields will become simpler after you practice writing your own SQL queries later in the program.


##### Endless possibilities of SQL
SQL statements are recommended to end with ; but some statements don't need it.

The WHERE clause narrows your query so that the database returns only the data with an exact value match or the data that matches a certain condition that you want to satisfy. 

For example, if you are looking for a specific customer with the last name Chavez, the WHERE clause would be: 

WHERE field1 = 'Chavez'


-> WHERE field1 LIKE 'Ch%' : filter the records where field1 started with Ch

###### Selection all columns :
Select * from table


*Comments* : -- for single line comment and /** */ for multiline also added with in a statement, if the other part of statement is on the next line


##### Aliases : 
You can also make it easier on yourself by assigning a new name or **alias** to the column or table names to make them easier to work with and avoid use of comments.

SELECT
my_table_alias.actual_column_name AS my_column_alias
FROM
actual_table_name AS my_table_alias

These aliases are good for the duration of the query only. An alias doesn’t change the actual name of a column or table in the database.


SELECT
*
FROM
Employee
WHERE
jobCode <> 'INT'
AND salary <= 30000;

<> means does not equal