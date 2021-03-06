### SQL: UPDATE Statement
**Description**
The SQL UPDATE statement is used to update existing records in the tables.

**Syntax**
The syntax for the UPDATE statement when updating a table in SQL is:
```
UPDATE table
SET column1 = expression1,
    column2 = expression2,
    ...
[WHERE conditions];
```
OR

The syntax for the SQL UPDATE statement when updating a table with data from another table is:
```
UPDATE table1
SET column1 = (SELECT expression1
               FROM table2
               WHERE conditions)
[WHERE conditions];
```

**Example - Update single column**
In this UPDATE example, we have a table called customers with the following data:

customer_id | last_name | first_name | favorite_website
-- | -- | -- | --
4000 | Jack | Joe | Guru99.com
5000 | Smith | Jane | digminecraft.com
6000 | Ferguson | Rebecca | Youtube.com
7000 | Reynolds | Allen | checkyourmath.com
8000 | Anderson | Paige | NULL
9000 | Jackson | Derek | Youtube.com

 Enter the following UPDATE statement:
```
UPDATE customers
SET first_name = 'Judy'
WHERE customer_id = 8000;
```
There will be 1 record updated. Select the data from the customers table again:
```
SELECT * FROM customers;
```
These are the results that you should see:

customer_id | last_name | first_name | favorite_website
-- | -- | -- | --
4000 | Jack | Joe | Guru99.com
5000 | Smith | Jane | digminecraft.com
6000 | Ferguson | Rebecca | Youtube.com
7000 | Reynolds | Allen | checkyourmath.com
8000 | Anderson | Judy | NULL
9000 | Jackson | Derek | Youtube.com

In this UPDATE example, the first_name field is set to 'Judy' in the customers table where the customer_id is equal to 8000.
