### Example - Greater Than Operator
You can use the > operator in SQL to test for an expression greater than.

In this example, we have a table called customers with the following data:

customer_id | last_name | first_name | favorite_website
-- | -- | -- | --
4000 | Jack | Joe | Guru99.com
5000 | Smith | Jane | digminecraft.com
6000 | Ferguson | Rebecca | Youtube.com
7000 | Reynolds | Allen | Gmail.com
8000 | Anderson | Paige | NULL

Enter the following SQL statement:
```
SELECT *
FROM customers
WHERE customer_id > 5000;
```
There will be 3 records selected. These are the results that you should see:

customer_id | last_name | first_name | favorite_website
-- | -- | -- | --
6000 | Ferguson | Rebecca | Youtube.com
7000 | Reynolds | Allen | Gmail.com
8000 | Anderson | Paige | NULL

