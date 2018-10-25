### Example - Greater Than or Equal Operator
In SQL, you can use the >= operator to test for an expression greater than or equal to.

Let's use the same customers table as the previous example.

customer_id | last_name | first_name | favorite_website
-- | -- | -- | --
4000 | Jack | Joe | Guru99.com
5000 | Smith | Jane | digminecraft.com
6000 | Ferguson | Rebecca | Youtube.com
7000 | Reynolds | Allen | Gmail.com
8000 | Anderson | Paige | NULL
9000 | Johnson | Derek | Youtube.com

Enter the following SQL statement:
```
SELECT *
FROM customers
WHERE customer_id >= 6000;
```
These are the results that you should see:

customer_id | last_name | first_name | favorite_website
-- | -- | -- | --
6000 | Ferguson | Rebecca | Youtube.com
7000 | Reynolds | Allen | Gmail.com
8000 | Anderson | Paige | NULL
9000 | Johnson | Derek | Youtube.com

In this example, the SELECT statement would return all rows from the customers table where the customer_id is greater than or equal to 6000. In this case, the supplier_id equal to 6000 would be included in the result set.

