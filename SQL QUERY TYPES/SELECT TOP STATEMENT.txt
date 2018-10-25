### SQL: SELECT TOP Statement
**Description**
The SQL SELECT TOP statement is used to retrieve records from one or more tables in a database and limit the number of records returned based on a fixed value or percentage.

**Syntax**
The syntax for the SELECT TOP statement in SQL is:
```
SELECT TOP (top_value) [ PERCENT ]
expressions
FROM tables
[WHERE conditions]
[ORDER BY expression [ ASC | DESC ]];
```

**Example - Using TOP keyword**
Let's look at a SQL example, where we use the TOP keyword in the SELECT statement.

For example:
```
SELECT TOP(5)
contact_id, last_name, first_name
FROM contacts
WHERE last_name = 'Anderson'
ORDER BY contact_id;
```
This SQL SELECT TOP example would select the first 5 records from the contacts table where the last_name is 'Anderson'. If there are other records in the contacts table that have a last_name of 'Anderson', they will not be returned by the SELECT statement.

**Example - Using TOP PERCENT keyword**
Let's look at a SQL example, where we use the TOP PERCENT keyword in the SELECT statement.

For example:
```
SELECT TOP(10) PERCENT
contact_id, last_name, first_name
FROM contacts
WHERE last_name = 'Anderson'
ORDER BY contact_id;
```
This SQL SELECT TOP example would select the first 10% of the records from the full result set. So in this example, the SELECT statement would return the top 10% of records from the contacts table where the last_name is 'Anderson'. The other 90% of the result set would not be returned by the SELECT statement.

