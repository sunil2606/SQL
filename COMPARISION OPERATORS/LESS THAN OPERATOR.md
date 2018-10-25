### Example - Less Than Operator
You can use the < operator in SQL to test for an expression less than.

In this example, we have a table called products with the following data:

product_id | product_name | category_id
-- | -- | --
1 | Pear | 50
2 | Banana | 50
3 | Orange | 50
4 | Apple | 50
5 | Bread | 75
6 | Sliced Ham | 25

Enter the following SQL statement:
```
SELECT *
FROM products
WHERE product_id < 5;
```
There will be 4 records selected. These are the results that you should see:

product_id | product_name | category_id
-- | -- | --
1 | Pear | 50
2 | Banana | 50
3 | Orange | 50
4 | Apple | 50

In this example, the SELECT statement would return all rows from the products table where the product_id is less than 5. A product_id equal to 5 would not be included in the result set.
