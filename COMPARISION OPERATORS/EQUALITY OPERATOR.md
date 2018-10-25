### Example - Equality Operator
In SQL, you can use the = operator to test for equality in a query.

In this example, we have a table called suppliers with the following data:


supplier_id | supplier_name | city | state
-- | -- | -- | --
100 | Microsoft | Redmond | Washington
200 | Google | Mountain View | California
300 | Oracle | Redwood City | California
400 | Kimberly-Clark | Irving | Texas


Enter the following SQL statement:
```
SELECT *
FROM suppliers
WHERE supplier_name = 'Microsoft';
```
There will be 1 record selected. These are the results that you should see:

supplier_id | supplier_name | city | state
-- | -- | -- | --
100 | Microsoft | Redmond | Washington

In this example, the SELECT statement above would return all rows from the suppliers table where the supplier_name is equal to Microsoft.

