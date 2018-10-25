### SELECT STATEMENT
**Description**
The SQL SELECT statement is used to retrieve records from one or more tables in your SQL database. The records retrieved are known as a result set.

**Syntax**
The syntax for the SELECT statement in SQL is:
```
SELECT expressions
FROM tables
[WHERE conditions]
[ORDER BY expression [ ASC | DESC ]];
```

**Parameters or Arguments**

**expressions**
The columns or calculations that you wish to retrieve. Use * if you wish to select all columns.

**tables**
The tables that you wish to retrieve records from. There must be at least one table listed in the FROM clause.

**WHERE conditions**
Optional. The conditions that must be met for the records to be selected. If no conditions are provided, then all records will be selected.

**ORDER BY expression**
Optional. The expression used to sort the records in the result set. If more than one expression is provided, the values should be comma separated.

**ASC**
Optional. ASC sorts the result set in ascending order by expression. This is the default behavior, if no modifier is provider.

**DESC**
Optional. DESC sorts the result set in descending order by expression.

**Example - Select All Fields from a Table**
Let's look at an example that shows how to use the SQL SELECT statement to select all fields from a table.

In this example, we have a table called customers with the following data:

customer_id | last_name | first_name | favorite_website
-- | -- | -- | --
4000 | Jack | Joe | Guru99.com
5000 | Smith | Jane | digminecraft.com
6000 | Ferguson | Rebecca | Youtube.com
7000 | Reynolds | Allen | checkyourmath.com
8000 | Anderson | Paige | NULL
9000 | Jackson | Derek | Youtube.com

Now let's demonstrate how the SELECT statement works by selecting all columns from the customers table. Enter the following SELECT statement:
```
SELECT *
FROM customers
WHERE favorite_website = 'Youtube.com'
ORDER BY last_name ASC;
```
There will be 2 records selected. These are the results that you should see:

customer_id | last_name | first_name | favorite_website
-- | -- | -- | --
6000 | Ferguson | Rebecca | Youtube.com
9000 | Jackson | Derek | Youtube.com


**Example - Select Individual Fields from a Table**

You can also use the SQL SELECT statement to select individual fields from the table, as opposed to all fields from the table.

In this example, we have a table called suppliers with the following data:

supplier_id | supplier_name | city | state
-- | -- | -- | --
100 | Microsoft | Redmond | Washington
200 | Google | Mountain View | California
300 | Oracle | Redwood City | California
400 | Kimberly-Clark | Irving | Texas
500 | Tyson Foods | Springdale | Arkansas
600 | SC Johnson | Racine | Wisconsin
700 | Dole Food Company | Westlake Village | California
800 | Flowers Foods | Thomasville | Georgia
900 | Electronic Arts | Redwood City | California

Now let's demonstrate how to use the SELECT statement to select individual columns from a table. Enter the following SELECT statement:
```
SELECT supplier_name, city
FROM suppliers
WHERE supplier_id > 500
ORDER BY supplier_name ASC, city DESC;
```

supplier_name | city
-- | --
Dole Food Company | Westlake Village
Electronic Arts | Redwood City
Flowers Foods | Thomasville
SC Johnson | Racine

This example would return only the supplier_name and city fields from the suppliers table where the supplier_id value is greater than 500. The results are sorted by supplier_name in ascending order and then city in descending order.



