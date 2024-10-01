# SQL-Basics-Lecture
SQL Basics Lecture with examples and queries.

Welcome to the **SQL Basics** lecture! This repository contains notes, SQL examples, and hands-on exercises to help you get started with SQL.

---

## Table of Contents:
1. [Introduction to Databases](#1-introduction-to-databases)
2. [Introduction to SQL](#2-introduction-to-sql)
3. [SQL Data Types and Commands](#3-sql-data-types-and-commands)
4. [Basic SQL Queries](#4-basic-sql-queries)
5. [Querying Data with Conditions](#5-querying-data-with-conditions)


---

## 1. Introduction to Databases

A **database** is a collection of interrelated data organized for easy access and management. Examples include databases for e-commerce websites, where user information, products, and orders are stored.

- **Database Management System (DBMS)**: A software application used to manage and interact with databases.
- **Relational Database Management System (RDBMS)**: Stores data in **tables** with rows (records) and columns (attributes), and allows you to manage relationships between different tables.

---

## 2. Introduction to SQL

**SQL** stands for **Structured Query Language** and is used to perform operations on relational databases. It enables users to:
- **C**REATE: Databases, tables, and insert data.
- **R**EAD: Retrieve data using queries.
- **U**PDATE: Modify existing data.
- **D**ELETE: Remove data from the database.

### Example:
```sql
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    salary DECIMAL(10, 2)
);
```
## 3. SQL Data Types and Commands
### SQL Data Types:
INT: Stores integer numbers.
VARCHAR(n): Stores text of variable length, where n is the maximum length.
DECIMAL(x, y): Stores decimal numbers with x digits total and y decimal places.
DATE: Stores date values.
### SQL Commands:
DDL (Data Definition Language): Commands like CREATE, ALTER, DROP that define the structure of the database.
DML (Data Manipulation Language): Commands like INSERT, UPDATE, DELETE that manipulate data.
DQL (Data Query Language): Commands like SELECT used to query and retrieve data.
### Example:
```sql
CREATE TABLE products (
    ProductID INT PRIMARY KEY,
    ProductName VARCHAR(50),
    Price DECIMAL(10, 2)
);

```
## 4. Basic SQL Queries
### Inserting Data:
```sql
INSERT INTO employees (id, name, salary)
VALUES (1, 'John Doe', 60000);

```
### Selecting Data:
```sql
SELECT * FROM employees;

```
### Updating Data:
```sql
UPDATE employees SET salary = 65000 WHERE id = 1;

```
### Deleting Data:
```sql
DELETE FROM employees WHERE id = 1;

```

## 5. Querying Data with Conditions (WHERE Clause)
The WHERE clause allows you to filter results based on conditions. 
### Example:

```sql
SELECT * FROM employees WHERE salary > 50000;
```
You can also use operators like:

#### = : Equal to
#### > : Greater than
#### < : Less than
#### != : Not equal to
