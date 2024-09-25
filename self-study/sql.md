# Basic SQL Commands

### SHOW
The `SHOW` command is used to display information about databases, tables, and other database objects.

**Example:**
```sql
SHOW DATABASES;
```
Output:
```
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mydatabase         |
| test               |
+--------------------+
```

### CREATE
The `CREATE` command is used to create a new database or table.

**Example:**
```sql
CREATE DATABASE mydatabase;
```
```sql
CREATE TABLE students (
    studentID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50)
);
```

### DROP
The `DROP` command is used to delete a database or table.

**Example:**
```sql
DROP DATABASE mydatabase;
```
```sql
DROP TABLE students;
```

### SELECT
The `SELECT` command is used to retrieve data from a database.

**Example:**
```sql
SELECT * FROM students;
```
Output:
```
+-----------+-----------+----------+
| studentID | FirstName | LastName |
+-----------+-----------+----------+
|         1 | John      | Doe      |
|         2 | Jane      | Smith    |
+-----------+-----------+----------+
```

### INSERT
The `INSERT` command is used to add new data to a table.

**Example:**
```sql
INSERT INTO students (studentID, FirstName, LastName)
VALUES (1, 'John', 'Doe');
```
