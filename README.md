# sql-challenge

## This project provides a database structure for an employee management system, including information about departments, employees, salaries, titles, and department management. The database is designed using an entity-relationship diagram (ERD) to visualize the connections between the various tables and relationships. The SQL scripts provided in the project help in creating the necessary tables and populating the data.

## 1. Project Files:
## Main 'EmployeeSQL' Folder ...
## QuickDBD-ERD.png : This is an image file of the Entity-Relationship Diagram (ERD) that visually represents the database structure.

## 'Data' Folder...
## 1.1 departments.csv : Contains the details about different departments within the organization.
## Columns:
### -- dept_no: Department number (Primary Key)
### -- dept_name: Name of the department
## 1.2 dept_emp.csv : Tracks the assignment of employees to departments.
## Columns:
### -- emp_no: Employee number (Foreign Key referencing employees)
### -- dept_no: Department number (Foreign Key referencing departments)
## 1.3 dept_manager.csv : Stores information about which employees manage which departments.
## Columns:
### -- dept_no: Department number (Foreign Key referencing departments)
### -- emp_no: Employee number (Foreign Key referencing employees)
## 1.4 employees.csv : Contains the basic details of employees in the organization.
## Columns:
### -- emp_no: Employee number (Primary Key)
### -- emp_title_id: Title of the employee (Foreign Key referencing titles)
### -- birth_date: Date of birth of the employee
### -- first_name: First name of the employee
### -- last_name: Last name of the employee
### -- sex: Gender of the employee
### -- hire_date: Date the employee was hired
## 1.5 salaries.csv : Records employee salaries.
## Columns:
### -- emp_no: Employee number (Foreign Key referencing employees)
### -- salary: Salary of the employee
## 1.6 titles.csv : Stores the titles or roles of employees.
## Columns:
### -- title_id: Title ID (Primary Key)
### -- title: Title description
## 'Queries' Folder...
### 1.7 HW_Tasks_Query.sql : This SQL file contains queries related to the various tasks required for managing and querying the database.
### 1.8 QuickDBD-Table_Schemata.sql : Contains the SQL statements for creating the table schema based on the ERD diagram.

## Project Structure:
### The project revolves around an employee management system where:

### Employees are assigned to departments, and some employees also manage those departments.
### Each employee has a unique employee number, and their details such as name, birthdate, and hire date are stored.
### Employees have specific roles/titles, and their corresponding salary is recorded.
### The relationships between employees, departments, and salaries are maintained via foreign key constraints, ensuring referential integrity across tables.
### How to Use:
### --Database Setup:
### ----Use the QuickDBD-Table_Schemata.sql to create the database schema. It contains the table definitions required to structure the employee management system.

### Data Insertion:
### -- The .csv files (like departments.csv, employees.csv, etc.) can be used to populate the corresponding tables with sample data using SQL import functionality.

## Task Queries:
## -- The HW_Tasks_Query.sql file contains queries to interact with the database. You can modify these queries to suit specific needs such as retrieving employee details, department managers, salary reports, etc.

## Visualization:
## -- The QuickDBD-ERD.png image provides a visual reference to the database structure, showing how tables relate to each other. This helps in understanding the relationships and designing queries effectively.
