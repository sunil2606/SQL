### Example - Inequality Operator
In SQL, there are two ways to test for inequality in a query. You can use either the <> or != operator. Both will return the same results.

Let's use the same suppliers table as the previous example.

supplier_id | supplier_name | city | state
-- | -- | -- | --
100 | Microsoft | Redmond | Washington
200 | Google | Mountain View | California
300 | Oracle | Redwood City | California
400 | Kimberly-Clark | Irving | Texas

Enter the following SQL statement to test for inequality using the <> operator:
```
SELECT *
FROM suppliers
WHERE supplier_name <> 'Microsoft';
```
OR enter this next SQL statement to use the != operator:
```
SELECT *
FROM suppliers
WHERE supplier_name != 'Microsoft';
```
There will be 8 records selected. These are the results you should see with either one of the SQL statements:

supplier_id | supplier_name | city | state
-- | -- | -- | --
200 | Google | Mountain View | California
300 | Oracle | Redwood City | California
400 | Kimberly-Clark | Irving | Texas

