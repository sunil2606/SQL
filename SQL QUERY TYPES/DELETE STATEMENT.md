### SQL: DELETE Statement
**Description**
The SQL DELETE statement is used to delete one or more records from a table.

**Syntax**
The syntax for the DELETE statement in SQL is:
```
DELETE FROM table
[WHERE conditions];
```

**Note**
- You do not need to list fields in the DELETE statement since you are deleting the entire row from the table.

**Example - DELETE Statement with One Condition**
If you run a DELETE statement with no conditions in the WHERE clause, all of the records from the table will be deleted.
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

```
DELETE FROM suppliers
WHERE supplier_name = 'Microsoft';
```
```
SELECT * FROM suppliers;
```
These are the results that you should see:

supplier_id | supplier_name | city | state
-- | -- | -- | --
200 | Google | Mountain View | California
300 | Oracle | Redwood City | California
400 | Kimberly-Clark | Irving | Texas
500 | Tyson Foods | Springdale | Arkansas
600 | SC Johnson | Racine | Wisconsin
700 | Dole Food Company | Westlake Village | California
800 | Flowers Foods | Thomasville | Georgia
900 | Electronic Arts | Redwood City | California

This example would delete all records from the suppliers table where the supplier_name is 'Microsoft'.
