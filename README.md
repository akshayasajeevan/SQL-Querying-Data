# Employee Database Management System | MySQL

## 📌 Overview

The **Employee Database Management System** is a MySQL project focused on querying and analyzing employee data stored in a relational database.

The project demonstrates SQL techniques for filtering, sorting, limiting, aggregating, grouping, and combining data from related tables.

---

## 🎯 Objectives

- Retrieve employee records using specific conditions.
- Apply the `WHERE` clause and SQL operators.
- Update missing employee information.
- Sort records using `ORDER BY`.
- Limit query results using `LIMIT`.
- Perform calculations using aggregate functions.
- Group records using `GROUP BY`.
- Filter grouped results using `HAVING`.
- Retrieve related information using SQL joins.

---

## 🗄️ Database Structure

The database consists of three related tables.

### Departments

Stores department information.

| Column | Description |
|---|---|
| `department_id` | Department identifier |
| `department_name` | Department name |

### Location

Stores location information.

| Column | Description |
|---|---|
| `location_id` | Location identifier |
| `location` | Location name |

### Employees

Stores employee information.

| Column | Description |
|---|---|
| `employee_id` | Employee identifier |
| `employee_name` | Employee name |
| `gender` | Employee gender |
| `age` | Employee age |
| `designation` | Job designation |
| `hire_date` | Hiring date |
| `department_id` | Department reference |
| `location_id` | Location reference |
| `salary` | Employee salary |

---

## 🔍 SQL Operations

### WHERE Clause & Operators

- Retrieve employees with a salary greater than ₹50,000 and hired before `2016-01-01`.
- Identify the employee with a missing designation.
- Update the missing designation to `Data Scientist`.

### ORDER BY

- Sort employees by department ID in ascending order.
- Sort salary in descending order.

### LIMIT

- Display the first five employees hired during 2018.

### Aggregate Functions

- Calculate the total salary of employees in the Finance department.
- Find the minimum age among all employees.

Functions used:

`SUM()` · `MIN()`

### GROUP BY

- Find the maximum salary for each location.
- Calculate the average salary for designations containing the word `Analyst`.

Functions used:

`MAX()` · `AVG()` · `GROUP BY` · `LIKE`

### HAVING

- Find departments with fewer than three employees.
- Find locations where female employees have an average age below 30.

Functions used:

`COUNT()` · `AVG()` · `HAVING`

---

## 🔗 SQL Joins

### INNER JOIN

Retrieves employee names, designations, and department names for employees assigned to departments.

### LEFT JOIN

Displays all departments along with the total number of employees, including departments with no employees.

### RIGHT JOIN

Displays all locations along with the employees assigned to each location. Locations without assigned employees return `NULL` for the employee name.

---

## 🛠️ Tools & Technologies

- **Database:** MySQL
- **SQL Client:** MySQL Workbench
- **Language:** SQL

---

## 📊 Database Records

| Data | Count |
|---|---:|
| Departments | 13 |
| Locations | 4 |
| Employees | 30 |

---

## 📁 Project Structure

```text
Employee-Database-Management-System/
│
├── Assignment_2_Querying_Data.sql
└── README.md
