# Employee_Management_System

A desktop-based Employee Management System built using Java Swing and MySQL Database. It allows adding, updating, deleting, and viewing employee records through an interactive GUI. Developed in NetBeans IDE with JDBC for database connectivity.

# Technology
1. Language: Java (Core)
2. GUI Framework: Java Swing / AWT
3. Database: MySQL
4. Connectivity: JDBC (Java Database Connectivity)
5. IDE: NetBeans

# Folder Structure

Employee_Management_System/
│
├── src/
│   ├── com/
│   │   └── employee/
│   │       ├── AddEmployee.java
│   │       ├── ViewEmployee.java
│   │       ├── UpdateEmployee.java
│   │       ├── RemoveEmployee.java
│   │       └── DatabaseConnection.java
│
├── lib/                # MySQL Connector JAR file
├── README.md           # Project Documentation
└── screenshots/        # Optional: images of the project UI

# Features
1. Add new employee details
2. View all employees in a table
3. Update existing records
4. Delete employee information
5. Login system for admin
6. Simple and user-friendly GUI

# Database Setup
1. Open MySQL Workbench or XAMPP phpMyAdmin.
2. Create a new database named:
   CREATE DATABASE employeemanagementsystem;
3. Select the database:
   USE employeemanagementsystem;
4. Create the login table:
   CREATE TABLE login (
    username VARCHAR(20),
    password VARCHAR(20)

};    
5. Insert admin login credentials:
  INSERT INTO login VALUES ('saini123', 's@12345');
6. Create the employee table:
   CREATE TABLE employee (
    name VARCHAR(20),
    fname VARCHAR(20),
    dob VARCHAR(30),
    salary VARCHAR(20),
    address VARCHAR(50)
);
7. Update the database connection in your Java file (if required):
   Connection con = DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/employeemanagementsystem", 
    "root", 
    ""
);

# How to Run the Project
1. Open NetBeans IDE.
2. Click File → Open Project and choose the folder of this project.
3. Make sure XAMPP is running and MySQL is started.
4. Open phpMyAdmin and import or create the database (as shown above).
5. In the project file, check this line:
   Connection con = DriverManager.getConnection("jdbc:mysql://localhost:3306/employeemanagementsystem", "root", "");
   Change username or password if needed.

6. Now click on the Run (green play) button in NetBeans.
7. The Employee Management System window will open.
8. Login and start managing employees — add, update, delete, or view records.

# Project Screenshots

### EMS
![EMS](screenshots/ems.png
