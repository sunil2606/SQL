### SQL: ORDER BY Clause
The SQL ORDER BY clause is used to sort the records in the result set for a SELECT statement.

**Syntax**
The syntax for the ORDER BY clause in SQL is:
```
SELECT expressions
FROM tables
[WHERE conditions]
ORDER BY expression [ ASC | DESC ];
```

Most programmers omit the ASC attribute if sorting in ascending order.

**Example - Sorting Results in descending order**
When sorting your result set in descending order, you use the DESC attribute in your ORDER BY clause. 


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

Enter the following SQL statement:
```
SELECT *
FROM suppliers
WHERE supplier_id > 400
ORDER BY supplier_id DESC;
```
There will be 5 records selected. These are the results that you should see:

supplier_id | supplier_name | city | state
-- | -- | -- | --
900 | Electronic Arts | Redwood City | California
800 | Flowers Foods | Thomasville | Georgia
700 | Dole Food Company | Westlake Village | California
600 | SC Johnson | Racine | Wisconsin
500 | Tyson Foods | Springdale | Arkansas


