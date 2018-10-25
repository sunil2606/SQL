### SQL: SELECT LIMIT Statement
**Description:**
The SQL SELECT LIMIT statement is used to retrieve records from one or more tables in a database and limit the number of records returned based on a limit value.
```
**TIP**: SELECT LIMIT is not supported in all SQL databases.
For databases such as SQL Server or MS Access, use the SELECT TOP statement to limit your results. The SELECT TOP statement is Microsoft's proprietary equivalent to the SELECT LIMIT statement.
```

**Syntax**
The syntax for the SELECT LIMIT statement in SQL is:
```
SELECT expressions
FROM tables
[WHERE conditions]
[ORDER BY expression [ ASC | DESC ]]
LIMIT number_rows [ OFFSET offset_value ];
```

**Example - Using LIMIT keyword**
Let's look at how to use a SELECT statement with a LIMIT clause in SQL.

For example:
```
SELECT contact_id, last_name, first_name
FROM contacts
WHERE website = 'Gmail.com'
ORDER BY contact_id DESC
LIMIT 5;
```
This SQL SELECT LIMIT example would select the first 5 records from the contacts table where the website is 'Gmail.com'. Note that the results are sorted by contact_id in descending order so this means that the 5 largest contact_id values will be returned by the SELECT LIMIT statement.
