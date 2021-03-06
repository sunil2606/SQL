### SQL FULL OUTER JOIN
Another type of join is called a SQL FULL OUTER JOIN. This type of join returns all rows from the LEFT-hand table and RIGHT-hand table with NULL values in place where the join condition is not met.

**Syntax**

The syntax for the SQL FULL OUTER JOIN is:
```
SELECT columns
FROM table1
FULL [OUTER] JOIN table2
ON table1.column = table2.column;
```

In some databases, the OUTER keyword is omitted and written simply as FULL JOIN.
