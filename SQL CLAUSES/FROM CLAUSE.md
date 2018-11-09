### SQL: FROM Clause

The SQL FROM clause is used to list the tables and any joins required for the SQL statement.

**Syntax**
The syntax for the FROM Clause in SQL is:
```
FROM table1
[ { INNER JOIN
  | LEFT [OUTER] JOIN
  | RIGHT [OUTER] JOIN
  | FULL [OUTER] JOIN } table2
ON table1.column1 = table2.column1 ]
```
**NOTE**
- When using the FROM clause in a SQL statement, there must be at least one table listed in the FROM clause.
- If there are two or more tables listed in the SQL FROM clause, these tables are generally joined using INNER or OUTER joins.


**Example - One Table Listed in the FROM Clause**

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
WHERE supplier_id < 400
ORDER BY city DESC;
```

supplier_id | supplier_name | city | state
-- | -- | -- | --
300 | Oracle | Redwood City | California
100 | Microsoft | Redmond | Washington
200 | Google | Mountain View | California

