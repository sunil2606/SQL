### SQL: DISTINCT Clause
The SQL DISTINCT clause is used to remove duplicates from the result set of a SELECT statement.

**Syntax**
The syntax for the DISTINCT clause in SQL is:
```
SELECT DISTINCT expressions
FROM tables
[WHERE conditions];
```

**Example - Finding Unique Values in a Column**


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
SELECT DISTINCT state
FROM suppliers
ORDER BY state;
```
There will be 6 records selected. These are the results that you should see:

state

--
Arkansas
California
Georgia
Texas
Washington
Wisconsin

