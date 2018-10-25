### SQL: INSERT Statement
**Description**
The SQL INSERT statement is used to insert a one or more records into a table. There are 2 syntaxes for the INSERT statement depending on whether you are inserting one record or multiple records.

**Syntax**
The syntax for the INSERT statement when inserting a single record in SQL is:
```
INSERT INTO table
(column1, column2, ... )
VALUES
(expression1, expression2, ... );
```
Or the syntax for the INSERT statement when inserting multiple records in SQL is:
```
INSERT INTO table
(column1, column2, ... )
SELECT expression1, expression2, ...
FROM source_tables
[WHERE conditions];
```

**Example - Using INSERT Statement to Insert One Record**
The simplest way use the INSERT statement is to insert one record into a table using the VALUES keyword. Let's look at an example of how to do this in SQL.

In this example, we have a table called categories with the following data:

category_id | category_name
-- | --
25 | Deli
50 | Produce
75 | Bakery
100 | General Merchandise
125 | Technology

Let's insert a new category record. Enter the following SQL statement:
```
INSERT INTO categories
(category_id, category_name)
VALUES
(150, 'Miscellaneous');
```
There will be 1 record inserted. Select the data from the categories table again:
```
SELECT * FROM categories;
```
These are the results that you should see:

category_id | category_name
-- | --
25 | Deli
50 | Produce
75 | Bakery
100 | General Merchandise
125 | Technology
150 | Miscellaneous

