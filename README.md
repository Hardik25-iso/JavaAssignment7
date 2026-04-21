# JavaAssignment7
---

# Student Record Manager (Java – File Handling System)

## Overview

This project is a **Java-based Student Record Management System** that uses **file handling** to store and manage student data persistently.

The application allows users to **add, view, update, and delete student records** through a menu-driven command-line interface. All records are stored in a text file, ensuring that data remains available even after the program terminates.

---

## Features

* Add new student records
* View all stored records in a formatted table
* Update existing student details
* Delete student records
* Persistent data storage using file handling
* Menu-driven interface for user interaction
* Error handling for invalid input and file operations

---

## Project Structure

### StudentRecordManager Class

This is the main and only class of the application.

Responsibilities:

* Handles all operations related to student records
* Manages file input/output operations
* Provides a menu-driven interface
* Ensures data validation and error handling

---

## Data Storage

* Records are stored in a file named:

```
students.txt
```

* Each record is stored in the following format:

```
RollNo,Name,Branch,Marks
```

Example:

```
101,Hardik,AI-ML,89.5
102,Rahul,CS,76.0
```

---

## Functionalities

### 1. Add Record

* Takes student details as input
* Appends the record to the file

### 2. View Records

* Reads all records from the file
* Displays them in a formatted table

### 3. Update Record

* Searches for a student using Roll Number
* Rewrites the file with updated details

### 4. Delete Record

* Removes a student record based on Roll Number
* Rewrites the file without the deleted record

---

## Application Workflow

1. User selects an option from the menu
2. Based on the choice:

   * Add → data is written to file
   * View → data is read and displayed
   * Update → file is modified
   * Delete → record is removed
3. Program continues until user exits

---

## How to Run the Program

### Prerequisites

* Java Development Kit (JDK) installed
* Terminal or Command Prompt

### Steps

1. Compile the program:

```
javac StudentRecordManager.java
```

2. Run the program:

```
java StudentRecordManager
```

---

## Sample Output

```
=== Student Record Manager ===

1.Add  2.View  3.Update  4.Delete  0.Exit
Choice: 1
Roll No : 101
Name    : Hardik
Branch  : AI-ML
Marks   : 90

Record added successfully.
```

---

## Concepts Used

* File Handling (BufferedReader, BufferedWriter, FileReader, FileWriter)
* Exception Handling (try-catch)
* Collections (`ArrayList`)
* String Manipulation
* Menu-driven programs
* Data persistence

---

## Error Handling

The program handles:

* Invalid numeric input (NumberFormatException)
* File not found scenarios
* General I/O errors
* Incorrect menu selections

---

