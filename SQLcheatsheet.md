# SQL Cheatsheet

## Basic SQL Commands

| Command | Description | Example |
|---------|-------------|---------|
| `SELECT` | Retrieves data from a table | `SELECT column1, column2 FROM table_name;` |
| `WHERE` | Filters records based on a condition | `SELECT * FROM table_name WHERE condition;` |
| `ORDER BY` | Sorts the result set in ascending or descending order | `SELECT * FROM table_name ORDER BY column1 DESC;` |
| `INSERT INTO` | Inserts new records into a table | `INSERT INTO table_name (column1, column2) VALUES (value1, value2);` |
| `UPDATE` | Modifies existing records in a table | `UPDATE table_name SET column1 = value1 WHERE condition;` |
| `DELETE` | Deletes records from a table | `DELETE FROM table_name WHERE condition;` |

## SQL Functions

| Function | Description | Example |
|----------|-------------|---------|
| `COUNT()` | Returns the number of rows | `SELECT COUNT(column_name) FROM table_name;` |
| `SUM()` | Returns the total sum of a numeric column | `SELECT SUM(column_name) FROM table_name;` |
| `AVG()` | Returns the average value of a numeric column | `SELECT AVG(column_name) FROM table_name;` |
| `MIN()` | Returns the smallest value of a column | `SELECT MIN(column_name) FROM table_name;` |
| `MAX()` | Returns the largest value of a column | `SELECT MAX(column_name) FROM table_name;` |

## SQL Joins

| Join Type | Description | Example |
|-----------|-------------|---------|
| `INNER JOIN` | Returns records with matching values in both tables | `SELECT column1, column2 FROM table1 INNER JOIN table2 ON table1.column_name = table2.column_name;` |
| `LEFT JOIN` (or `LEFT OUTER JOIN`) | Returns all records from the left table, and the matched records from the right table | `SELECT column1, column2 FROM table1 LEFT JOIN table2 ON table1.column_name = table2.column_name;` |
| `RIGHT JOIN` (or `RIGHT OUTER JOIN`) | Returns all records from the right table, and the matched records from the left table | `SELECT column1, column2 FROM table1 RIGHT JOIN table2 ON table1.column_name = table2.column_name;` |
| `FULL JOIN` (or `FULL OUTER JOIN`) | Returns all records when there is a match in either left or right table | `SELECT column1, column2 FROM table1 FULL JOIN table2 ON table1.column_name = table2.column_name;` |

## SQL Clauses & Operators

| Clause/Operator | Description | Example |
|-----------------|-------------|---------|
| `GROUP BY` | Groups rows with the same values | `SELECT column1, COUNT(column2) FROM table_name GROUP BY column1;` |
| `HAVING` | Filters the result of a `GROUP BY` | `SELECT column1, COUNT(column2) FROM table_name GROUP BY column1 HAVING COUNT(column2) > value;` |
| `LIKE` | Searches for a specified pattern | `SELECT * FROM table_name WHERE column_name LIKE 'pattern%';` |
| `IN` | Specifies multiple values in a `WHERE` clause | `SELECT * FROM table_name WHERE column_name IN (value1, value2);` |
| `BETWEEN` | Selects values within a range | `SELECT * FROM table_name WHERE column_name BETWEEN value1 AND value2;` |
| `NOT` | Negates a condition | `SELECT * FROM table_name WHERE NOT column_name = value;` |
| `AND` & `OR` | Combines multiple conditions | `SELECT * FROM table_name WHERE condition1 AND condition2;` |

## Advanced SQL Concepts

| Concept | Description | Example |
|---------|-------------|---------|
| Subqueries | A query inside another query | `SELECT column_name FROM table_name WHERE column_name = (SELECT column_name FROM another_table);` |
| Indexes | Used to retrieve data from the database more quickly | `CREATE INDEX index_name ON table_name (column_name);` |
| Transactions | A sequence of SQL operations executed as a single unit | `BEGIN TRANSACTION; SQL_statement1; SQL_statement2; COMMIT;` |
| Views | A virtual table based on the result set of an SQL statement | `CREATE VIEW view_name AS SELECT column1, column2 FROM table_name WHERE condition;` |

---

**Note**: This cheatsheet provides a concise overview of common SQL commands and concepts. Always refer to specific database documentation for detailed information and nuances.

