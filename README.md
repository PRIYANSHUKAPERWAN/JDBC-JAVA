JDBC Assignment Overview

This project demonstrates how to use Java Database Connectivity (JDBC) to interact with a MySQL database. It is divided into three main parts:

Connecting to MySQL and Fetching Data

Performing CRUD Operations on a Product Table

Building a Student Management System using JDBC and MVC Architecture

Part A: Connecting to MySQL and Fetching Data Description

Establishes a connection between Java and MySQL using JDBC.

Executes a SELECT query to retrieve records from a table.

Key Concepts

DriverManager

Connection

Statement

ResultSet

Command Example SELECT * FROM employees;

Part B: CRUD Operations on Product Table Description

Implements Create, Read, Update, and Delete operations on a product table using JDBC.

Features

Add new product

View all products

Update product details

Delete a product

Technologies Used

Java 8+

MySQL Database

JDBC API

Sample Table Structure CREATE TABLE product ( id INT PRIMARY KEY AUTO_INCREMENT, name VARCHAR(50), price DOUBLE );

Part C: Student Management Application (JDBC + MVC) Description

A mini console-based application that manages student records using MVC architecture and JDBC.

Architecture StudentApp/ ├── model/ │ └── Student.java ├── dao/ │ └── StudentDAO.java ├── controller/ │ └── StudentController.java └── Main.java

Modules

Model: Defines Student class.

DAO: Handles database operations using JDBC.

Controller: Manages user input and application flow.

Sample Table CREATE TABLE student ( id INT PRIMARY KEY, name VARCHAR(50), age INT );

Setup Instructions

Install MySQL and create a database (e.g., testdb).

Update credentials in each Java file:

String url = "jdbc:mysql://localhost:3306/testdb"; String user = "root"; String password = "yourpassword";

Compile and run:

javac *.java java Main

Ensure MySQL JDBC driver (mysql-connector-j.jar) is added to your classpath.

Learning Outcomes

Understand database connectivity in Java.

Implement CRUD operations using JDBC.

Learn MVC architecture with database interaction.

Use PreparedStatement for secure SQL queries.

Author

Priyanshu kaperwan Computer Science Engineering, Chandigarh University

