# 🧑‍💼 Employee Management System

A Java-based GUI desktop application that allows you to manage employee records efficiently. Built using **Java Swing** for the interface and **MySQL** for database operations.

---

## 📌 Features

- 🔐 Secure login system  
- ➕ Add new employee records  
- 👁️ View all employee details  
- 📝 Update existing employee data  
- ❌ Delete employee records  
- 🗃️ JDBC connectivity with MySQL  
- 📅 Integrated calendar (via jCalendar)

---

## 🛠️ Tech Stack

- **Language**: Java  
- **Frontend**: Java Swing  
- **Backend**: MySQL  
- **Libraries**:
  - `jcalendar-1.4.jar`
  - `rs2xml.jar`
- **IDE Recommended**: IntelliJ IDEA / Eclipse  
- **Build Tool**: Manual via terminal or IDE

---

## 🧑‍💻 How to Run the Application

### 1. Clone the Repository

```bash

2. Set Up the MySQL Database
Open MySQL and create a database, e.g., employeedb
Create a table with suitable schema (columns like name, age, address, etc.)
Update your conn.java file with your DB name, username, and password:



git clone https://github.com/Subhangi69/Employee-Management-System.git
cd Employee-Management-System

## 2. Set Up the MySQL Database
### Open MySQL and run the following commands to create the database and table:

CREATE DATABASE IF NOT EXISTS employeedb;
USE employeedb;

CREATE TABLE employee (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  age INT,
  address VARCHAR(255),
  salary DOUBLE
  -- Add more columns as per your application
);

### 2.Update your conn.java file with your database name, username, and password:
Connection c = DriverManager.getConnection(
  "jdbc:mysql://localhost:3306/employeedb", 
  "root", 
  "your_password"
);

## 3. Compile the Project
### Navigate to the src directory and run:

javac -cp ".;../libraries/jcalendar-1.4.jar;../libraries/rs2xml.jar" employee/management/system/*.java

##  4. Run the Application

java -cp ".;../libraries/jcalendar-1.4.jar;../libraries/rs2xml.jar" employee.management.system.Splash


## The application will launch with a splash screen and then take you to the login window.

