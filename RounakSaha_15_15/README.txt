# PROJECT OUTLINE

This project is a command-line Coaching Centre System developed using Java and MySQL.
It allows users to manage student enrolments and fee payments through a set of text interfaces.

The system supports enrolling students, recording fee payments, viewing batch students, and tracking fee defaulters.

---

## FEATURES

### 1. Enrol Student
- Enrol new students and assign them to a specific batch.
- Requires student name, phone number, and batch ID.

### 2. Record Fee Payment
- Record a fee payment for a specific month.
- Requires student ID and payment month (YYYY-MM).

### 3. View Batch Students
- View all students enrolled in a specific batch.
- Displays student ID, name, and phone number.

### 4. Fee Defaulters
- Displays students who haven't paid their fees for a specific month.

---

## TECHNOLOGIES USED

- Java (JDK 8 or newer)
- MySQL Database
- JDBC (MySQL Connector/J)

---

## PROJECT STRUCTURE

`src/Main.java`
- Main execution flow (Menu Interface)

`src/DBConnection.java`
- Handles database connection using JDBC

`sql/schema.sql`
- SQL file to create database and tables

---

## DATABASE SETUP

1. Open MySQL Workbench or Command Line.
2. Run the following SQL:

CREATE DATABASE coaching_centre;
USE coaching_centre;
[Create Tables as defined in sql/schema.sql]

---

## HOW TO RUN THE PROJECT

1. Clone the repository or download the source code.
2. Ensure MySQL is running.
3. Compile:
  javac -cp ".;lib/mysql-connector-j-8.x.x.jar" src/*.java

4. Run:
  java -cp "src;lib/mysql-connector-j-8.x.x.jar" Main

---

## FUTURE ENHANCEMENTS

- Develop a Graphical User Interface (GUI) using JavaFX or Swing.
- Implement user authentication with different roles (Admin/Student).
- Automate receipt generation for fee payments.
- Add SMS or email notifications for fee defaulters.

---

## AUTHOR

Name: Rounak Saha
Course: MCA
Project: Coaching Centre System

---

## END OF FILE