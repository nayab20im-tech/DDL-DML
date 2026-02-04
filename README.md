# Database Systems Lab - Assignment 02 (DDL & DML)

## Project Overview
[cite_start]This repository contains the solution for **Assignment 02** of the Database Systems Lab course at **GIFT University**[cite: 23, 24]. [cite_start]The project focuses on utilizing **DDL (Data Definition Language)** to create a relational database schema and **DML (Data Manipulation Language)** to populate and modify the data[cite: 35, 39, 50].

## Course Information
* [cite_start]**University:** GIFT University, Gujranwala [cite: 23, 26]
* [cite_start]**Course:** Database Systems-Lab (CS-146L) [cite: 28]
* [cite_start]**Instructor:** Dilawar Abbas [cite: 30]
* [cite_start]**Topic:** DDL + DML (Constraints, Insertions, and Alterations) [cite: 35]

---

## Assignment Tasks

### Question 1: Database Creation (DDL) & Insertion (DML)
[cite_start]The first task involved creating three related tables with appropriate **Primary Key** and **Foreign Key** constraints, followed by inserting 5-6 records into each table[cite: 39, 50, 51].

#### 1. Faculty Table
* [cite_start]**Attributes:** `facultyID` (PK), `facultyName`, `Email`, `Department`[cite: 42].
* [cite_start]**Data:** Populated with faculty members from Computer Science, Electrical Engineering, and Mathematics departments[cite: 4, 6, 7].

#### 2. Students Table
* [cite_start]**Attributes:** `StudentID` (PK), `StudentName`, `Email`, `EnrollmentYear`, `FacultyID` (FK)[cite: 44].
* [cite_start]**Relationship:** Linked to the Faculty table via `FacultyID`[cite: 2].

#### 3. Projects Table
* [cite_start]**Attributes:** `ProjectID` (PK), `ProjectTitle`, `Description`, `StudentID` (FK), `FacultyID` (FK)[cite: 46].
* [cite_start]**Relationship:** Linked to both Students and Faculty tables to track project supervision and assignment[cite: 3].

### Question 2: Table Alteration
The second task required updating the schema of the `students` table.
* [cite_start]**Query:** Renamed the column `"Email"` to `"Students_email"` using the `ALTER TABLE` command[cite: 22, 53].

---

## Database Schema & Relationships
The database enforces the following relationships:
* **One-to-Many:** One Faculty member can supervise multiple Students (implied by FK in Students table).
* **Project Assignment:** Projects are linked to specific Students and supervising Faculty members.

---

## Output Screenshots
Below are the screenshots of the tables after executing the DDL and DML queries.

### Faculty Table Data
![Faculty Table](Faculty%20Table.jpg)

### Students Table Data
![Students Table](Students%20Table.jpg)

### Projects Table Data
![Projects Table](Projects%20Table.jpg)

### Structure Change (Q2 Output)
*Showing the renamed `Students_email` column.*
![Q2 Structure Output](Q2_Output%20Screenshot.jpg)

---

## How to Run
1.  Open your SQL environment (e.g., phpMyAdmin, MySQL Workbench).
2.  Copy the SQL script provided in `queries.txt`.
3.  Execute the queries in the following order:
    1.  Table Creation (Faculty -> Students -> Projects).
    2.  Data Insertion.
    3.  Alter Table command.

---

## Author
* **Name:** [Your Name]
* **Roll Number:** [Your Roll Number]
* **Section:** [Your Section]
