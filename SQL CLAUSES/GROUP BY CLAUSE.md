### SQL: GROUP BY Clause

The SQL GROUP BY clause can be used in a SELECT statement to collect data across multiple records and group the results by one or more columns.

**Syntax**
The syntax for the GROUP BY clause in SQL is:
```
SELECT expression1, expression2, ... expression_n, 
       aggregate_function (aggregate_expression)
FROM tables
[WHERE conditions]
GROUP BY expression1, expression2, ... expression_n
[ORDER BY expression [ ASC | DESC ]];
```

**Example - Using GROUP BY with the SUM Function**

employee_number | last_name | first_name | salary | dept_id
-- | -- | -- | -- | --
1001 | Smith | Sam | 62000 | 500
1002 | Doe | Jane | 57500 | 500
1003 | Pitt | Brad | 71000 | 501
1004 | Sparrow | Jack | 42000 | 501

Enter the following SQL statement:
```
SELECT dept_id, SUM(salary) AS total_salaries
FROM employees
GROUP BY dept_id;
```
There will be 2 records selected. These are the results that you should see:

dept_id | total_salaries
-- | --
500 | 119500
501 | 113000


**Example - Using GROUP BY with the MIN function**

employee_number | last_name | first_name | salary | dept_id
-- | -- | -- | -- | --
1001 | Smith | Sam | 62000 | 500
1002 | Doe | Jane | 57500 | 500
1003 | Pitt | Brad | 71000 | 501
1004 | Sparrow | Jack | 42000 | 501

Enter the following SQL statement:
```
SELECT dept_id, MIN(salary) AS lowest_salary
FROM employees
GROUP BY dept_id;
```
There will be 2 records selected. These are the results that you should see:

dept_id | lowest_salary
-- | --
500 | 57500
501 | 42000

