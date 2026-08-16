# School Management System

A console-based **School Management System** developed in C++ for managing basic student records. The project provides a simple menu-driven interface that allows users to add, view, search, update, and delete student information.

This project focuses on practicing fundamental C++ programming concepts and implementing a basic student record management system.

## Features

* Add multiple student records
* View all student records
* Search for a student by roll number
* Update existing student information
* Delete student records
* Display the total number of students
* Validate menu choices
* Simple and easy-to-use console interface

## Student Information

The system stores the following information for each student:

* Name
* Roll Number
* Section
* Age

## Menu Options

```text
===== SCHOOL MANAGEMENT SYSTEM =====
1. Add Student
2. View Students
3. Search Student
4. Update Student
5. Delete Student
6. Total Students
7. Exit
```

### 1. Add Student

Allows the user to add one or multiple students to the system. For each student, the program collects their name, roll number, section, and age.

### 2. View Students

Displays the complete information of all students currently stored in the system.

### 3. Search Student

Searches for a student using their roll number. If the student exists, their complete record is displayed.

### 4. Update Student

Allows the user to update the information of an existing student by searching for their roll number.

### 5. Delete Student

Deletes a student record using their roll number. After deletion, the remaining records are shifted to maintain the order of the array.

### 6. Total Students

Displays the current total number of students stored in the system.

### 7. Exit

Terminates the program and displays an exit message.

## Technologies Used

* **Language:** C++
* **Library:** Standard C++ Library
* **Interface:** Command Line / Console

## C++ Concepts Used

This project demonstrates several fundamental programming concepts, including:

* Structures (`struct`)
* Arrays
* Functions
* Variables and data types
* Conditional statements
* `for` and `while` loops
* Boolean variables
* User input and output
* Linear searching
* Record updating
* Array element shifting
* Basic input validation

## Data Structure

Student records are stored using a C++ structure:

```cpp
struct student {
    string name;
    int rollno;
    string section;
    int age;
};
```

The program then stores these structures in a fixed-size array:

```cpp
student info[100];
```

The current implementation can therefore store up to **100 student records** during a single execution of the program.

## How the Delete Function Works

When a student is deleted, the program searches for the student's roll number. Once the record is found, every record after it is shifted one position to the left.

For example:

```text
Before deletion:

Student 1
Student 2
Student 3
Student 4

Delete Student 2

After deletion:

Student 1
Student 3
Student 4
```

This allows the program to keep the student records together without leaving an empty position in the middle of the array.

## Limitations

This is a basic console-based implementation, so it currently has some limitations:

* Maximum capacity of 100 students
* Student data is stored only in memory
* Data is lost when the program is closed
* No database or file storage
* Duplicate roll numbers are not prevented
* Input validation is limited
* No graphical user interface

## Future Improvements

The project can be further developed by adding:

* File handling for permanent data storage
* Database integration
* Duplicate roll number detection
* Improved input validation
* Student sorting
* Attendance management
* Marks and grade management
* Teacher management
* Login/authentication system
* Object-oriented programming using classes
* A graphical user interface

## Purpose of the Project

The purpose of this project is to develop a practical understanding of **C++ fundamentals and basic data management** by building a functional student management system.

It serves as a foundation for developing more advanced applications using **Object-Oriented Programming, file handling, databases, and user authentication**.

## Author

**Muhammad Talha Zahid**

GitHub: [talhazahid-1234](https://github.com/talhazahid-1234)

---

If you find this project useful or have suggestions for improvement, feel free to explore the repository and contribute.
