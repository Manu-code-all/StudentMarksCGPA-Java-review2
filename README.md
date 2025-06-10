Student Management System
Description
A console-based application developed in Java to manage student records. This project allows users to perform CRUD operations (Create, Read, Update, Delete) on student data, search students by name, and persist data to a file (students.txt). It includes robust input validation, error handling, and a modular design for better component integration.
Features

Add a new student with details: ID, name, age, and grade.
View all students in the system.
Update an existing student's details by ID.
Delete a student by ID.
Search for students by partial name matches (innovative feature).
Data persistence using a text file (students.txt).
Comprehensive input validation (e.g., unique IDs, valid names, age, and grade ranges).
Error handling to prevent crashes from invalid inputs.
User-friendly console menu with clear feedback.

How to Run

Ensure you have Java installed on your system (JDK 8 or higher recommended).
Open a terminal or command prompt and navigate to the project directory.
Compile the project:javac Main.java

This will compile all Java files in the project.
Run the program:java Main

The program will start, and you’ll see the main menu in the console.

Usage

Upon running the program, you’ll see the following menu:Student Management System
1. Add Student
2. View All Students
3. Update Student
4. Delete Student
5. Search Student by Name
0. Exit
Enter your choice:


Select an option by entering a number (0–5) and pressing Enter.
Follow the prompts for each operation:
Add Student: Enter a unique ID (positive integer), name (letters and spaces only), age (5–100), and grade (0–100).
View All Students: Displays all student records.
Update Student: Enter the ID of the student to update, then provide new details.
Delete Student: Enter the ID of the student to delete.
Search Student by Name: Enter a name (or part of a name) to search for matching students.
Exit: Saves all data to students.txt and exits the program.


The program includes validation:
ID must be a unique positive integer.
Name must contain only letters and spaces (e.g., John Doe).
Age must be between 5 and 100.
Grade must be between 0 and 100.


If you enter invalid data, you’ll see an error message (e.g., Invalid input. Please try again.) and return to the menu.

Example Interaction
Enter your choice: 1
Enter student ID: 101
Enter student name: John Doe
Enter student age: 20
Enter student grade: 85.5
Student added successfully!

Enter your choice: 2
ID: 101, Name: John Doe, Age: 20, Grade: 85.5

Enter your choice: 0
Exiting... Data saved.

File Structure

data/
FileHandler.java: Manages reading and writing student data to students.txt.
students.txt: Stores student data in the format ID,name,age,grade.


models/
Student.java: Defines the Student class with attributes (ID, name, age, grade).


services/
StudentService.java: Handles student operations (add, view, update, delete, search).
AdminService.java: Placeholder for admin-specific features (e.g., viewing all students).


utils/
Validator.java: Validates user inputs (ID, name, age, grade).


Main.java: Entry point of the program, providing the console-based menu interface.
README.md: Project documentation (this file).

Notes

The program automatically loads student data from students.txt when it starts and saves changes to the file when you exit.
If students.txt does not exist, it will be created automatically when you add a student.
Ensure your terminal has write permissions in the project directory to create and modify students.txt.

