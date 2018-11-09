### SQL: WHERE Clause
The SQL WHERE clause is used to filter the results and apply conditions in a SELECT, INSERT, UPDATE, or DELETE statement.

**Syntax**
The syntax for the WHERE clause in SQL is:
```
WHERE conditions;
```

**Example - One Condition in the WHERE Clause**


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
WHERE state = 'California';
```
These are the results that you should see:

supplier_id | supplier_name | city | state
-- | -- | -- | --
200 | Google | Mountain View | California
300 | Oracle | Redwood City | California
700 | Dole Food Company | Westlake Village | California
900 | Electronic Arts | Redwood City | California

