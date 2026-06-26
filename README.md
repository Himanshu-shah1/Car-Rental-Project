

 🚗 Car Rental Management System
 
📌 Project Overview

The **Car Rental Management System** is a database management project developed using **MySQL and SQL** to automate and streamline the operations of a car rental business. The project provides an efficient way to manage customer information, vehicle inventory, rental bookings, payment records, and vehicle availability through a structured relational database.

This project demonstrates practical implementation of **Database Management System (DBMS)** concepts, including database design, normalization, relationships, constraints, and advanced SQL queries. The system is designed to reduce manual record-keeping, improve data accuracy, and enable faster access to business information.

The database maintains records of customers, vehicles, rentals, and payments while ensuring data integrity through primary and foreign key relationships. SQL queries are used to perform CRUD operations, generate reports, and analyze rental business performance.

---

## 🎯 Objectives

* Manage customer and vehicle information efficiently.
* Track vehicle bookings and rental transactions.
* Monitor vehicle availability and rental status.
* Store payment and billing records securely.
* Generate reports for business analysis and decision-making.
* Demonstrate practical SQL and database management skills.

---

## 🛠 Technologies Used

* MySQL
* SQL
* MySQL Workbench
* Git
* GitHub

---

## 📂 Database Components

### Customer Table

Stores customer details such as:

* Customer ID
* Name
* Contact Information
* Address

### Car Table

Stores vehicle information:

* Car ID
* Vehicle Name
* Brand
* Model
* Rental Price
* Availability Status

### Booking Table

Stores booking details:

* Booking ID
* Customer ID
* Car ID
* Booking Date
* Rental Duration

### Payment Table

Stores payment information:

* Payment ID
* Booking ID
* Amount
* Payment Date
* Payment Method

---

## 💡 SQL Concepts Implemented

* CREATE TABLE
* ALTER TABLE
* INSERT
* UPDATE
* DELETE
* SELECT
* WHERE Clause
* ORDER BY
* GROUP BY
* Aggregate Functions
* INNER JOIN
* LEFT JOIN
* RIGHT JOIN
* Subqueries
* Views
* Stored Procedures
* Triggers
* Constraints

  * Primary Key
  * Foreign Key
  * NOT NULL
  * UNIQUE

---

## 📊 Key Features

* Customer Management
* Vehicle Inventory Management
* Rental Booking System
* Payment Tracking
* Vehicle Availability Monitoring
* Revenue Analysis
* Rental History Tracking
* Business Reporting

---

# ⚙️ Installation Guide

## Windows 11 Setup

### Step 1: Install MySQL Server

Download and install MySQL Community Server:

[MySQL Community Downloads](https://dev.mysql.com/downloads/?utm_source=chatgpt.com)

During installation:

* Select Developer Default
* Install MySQL Server
* Install MySQL Workbench
* Configure root password
* Complete installation

### Step 2: Verify Installation

Open Command Prompt:

```bash
mysql -u root -p
```

Enter your MySQL password.

If MySQL starts successfully, installation is complete.

### Step 3: Clone GitHub Repository

```bash
git clone https://github.com/Himanshu-shah1/Car-Rental-Project.git
```

Move into project directory:

```bash
cd Car-Rental-Project
```

### Step 4: Open MySQL Workbench

1. Launch MySQL Workbench
2. Connect to Local MySQL Server
3. Open the SQL script from the project folder
4. Execute the script

### Step 5: Create Database

```sql
CREATE DATABASE car_rental_db;
USE car_rental_db;
```

### Step 6: Import SQL File

Open and execute the project's SQL file:

```sql
SOURCE car_rental.sql;
```

---

# 🍎 macOS Setup

## Step 1: Install Homebrew

Open Terminal and run:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Step 2: Install MySQL

```bash
brew install mysql
```

## Step 3: Start MySQL Service

```bash
brew services start mysql
```

## Step 4: Verify Installation

```bash
mysql --version
```

## Step 5: Login to MySQL

```bash
mysql -u root -p
```

## Step 6: Clone Repository

```bash
git clone https://github.com/Himanshu-shah1/Car-Rental-Project.git
```

Navigate to project directory:

```bash
cd Car-Rental-Project
```

## Step 7: Import Database

```bash
mysql -u root -p < car_rental.sql
```

---

## ▶️ Running the Project

Open MySQL and execute:

```sql
USE car_rental_db;
SHOW TABLES;
```

Verify that all tables are created successfully.

Example:

```sql
SELECT * FROM Customers;
SELECT * FROM Cars;
SELECT * FROM Bookings;
SELECT * FROM Payments;
```

---

## 📈 Sample Analysis Queries

### Total Revenue Generated

```sql
SELECT SUM(amount) AS Total_Revenue
FROM Payments;
```

### Most Frequently Rented Vehicle

```sql
SELECT Car_ID, COUNT(*) AS Rental_Count
FROM Bookings
GROUP BY Car_ID
ORDER BY Rental_Count DESC;
```

### Customer Booking Analysis

```sql
SELECT Customer_ID,
COUNT(*) AS Total_Bookings
FROM Bookings
GROUP BY Customer_ID;
```

---

## 🎓 Learning Outcomes

Through this project, I gained hands-on experience in:

* Relational Database Design
* Database Normalization
* SQL Query Development
* Data Management
* Data Analysis
* Report Generation
* Business Intelligence Concepts
* Problem Solving and Analytical Thinking

---

## 🔗 GitHub Repository


