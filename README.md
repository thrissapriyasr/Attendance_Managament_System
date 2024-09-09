# Student Attendance Management System

This is a simple **Student Attendance Management System** built using **Java Swing** for the GUI (Graphical User Interface) and **MySQL** as the backend database. The system allows users to add, update, and view students' attendance records.

## Features

- **Add Attendance Record**: Users can enter the student's name, subject, total number of classes, and the number of attended classes. The system calculates the attendance percentage and stores the information in the database.
- **Update Attendance Record**: Users can update existing attendance records based on the selected student and subject.
- **Display Attendance Records**: A table displays all student attendance records fetched from the MySQL database.
- **Select & Edit Record**: Users can select a record from the table to edit the attendance details.

## Technology Stack

- **Java (Swing)**: For the GUI components like text fields, buttons, and tables.
- **MySQL**: Database to store attendance records.
- **JDBC**: For connecting the Java application to the MySQL database.

## Prerequisites

To run this project, you'll need:

1. **Java Development Kit (JDK)**: Ensure you have JDK installed on your system.
2. **MySQL Database**: Install MySQL and create a database named `intern`.
3. **MySQL Connector for Java**: Ensure the MySQL JDBC driver (`mysql-connector-java`) is added to your project.

## Database Setup

1. Create a database named `intern` in your MySQL server:
    ```sql
    CREATE DATABASE intern;
    ```

2. Create a table named `attendance`:
    ```sql
    CREATE TABLE attendance (
        id INT PRIMARY KEY AUTO_INCREMENT,
        NAME VARCHAR(50),
        SUBJECT VARCHAR(50),
        TOTAL_CLASSES INT,
        CLASSES_ATTENDED INT,
        TOTAL_ATTENDANCE VARCHAR(10)
    );
    ```

## How to Run

1. Clone the repository or download the source code.
2. Open the project in your favorite Java IDE (like IntelliJ IDEA or Eclipse).
3. Add the **MySQL JDBC Driver** (`mysql-connector-java`) to your project classpath.
4. Make sure your MySQL server is running, and you have the `intern` database set up.
5. Run the `Main` class to start the application.

## Usage

- **Add Record**: Fill in the student's name, subject, total classes, and attended classes. Click the **ADD RECORD** button to save the data.
- **Update Record**: Select a student record from the table, modify the classes attended, and click the **UPDATE RECORD** button to update the record.
- **Table Interaction**: Click on any row in the table to edit that specific record.

## Code Explanation

- **Main.java**: The entry point of the program. It creates an instance of the `Attendance` class to launch the application.
- **Attendance.java**: This class contains the GUI and database interaction logic:
  - Handles adding and updating attendance records.
  - Connects to MySQL to perform database operations.
  - Displays attendance data in a table.

## Screenshots

![image](https://github.com/user-attachments/assets/d4928d23-f4d3-4639-ad72-6833c9a009ae)





