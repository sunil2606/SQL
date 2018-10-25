### Example - Less Than or Equal Operator
In SQL, you can use the <= operator to test for an expression less than or equal to.

Let's use the same products table as the previous example.

product_id | product_name | category_id
-- | -- | --
1 | Pear | 50
2 | Banana | 50
3 | Orange | 50
4 | Apple | 50
5 | Bread | 75
6 | Sliced Ham | 25

Enter the following SQL statement
```
SELECT *
FROM products
WHERE product_id <= 5;
```
There will be 5 records selected. These are the results that you should see:

product_id | product_name | category_id
-- | -- | --
1 | Pear | 50
2 | Banana | 50
3 | Orange | 50
4 | Apple | 50
5 | Bread | 75

