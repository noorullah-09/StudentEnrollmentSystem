# StudentEnrollmentSystem
Student Enrollment System that manages information about students and the courses they are enrolled in. The system should be able to handle multiple students and courses.

The provided code represents a simple Java program for a student management system. This system allows users to input information about students and the courses they are enrolled in. The data is then stored in a MySQL database.

Here's a brief description of the key components and functionalities:

1. **Student Class (`Student.java`):**
   - Represents a student with attributes such as name, roll number, and a list of enrolled courses.
   - Provides methods for enrolling students in courses and displaying student information.

2. **Course Class (`Course.java`):**
   - Represents a course with attributes like course code, name, and credits.
   - Provides a method to display course information.

3. **MainStudentManagement Class (`MainStudentManagement.java`):**
   - The main class that contains the `main` method to run the program.
   - Establishes a connection to a MySQL database using JDBC for data storage.
   - Utilizes `Scanner` for user input.
   - Prompts the user to enter details for multiple students, including their names, roll numbers, and courses.
   - Handles input validation for student roll numbers and gracefully manages invalid inputs.
   - Displays information about students and courses after input.
   - Inserts the entered data into the MySQL database, specifically into tables named `student4`, `course4`, and `enrollment`.
   - Utilizes prepared statements to prevent SQL injection.

4. **Database Schema:**
   - The code assumes the existence of a MySQL database named `day4` with tables `student4`, `course4`, and `enrollment`.
   - The tables store information about students, courses, and the enrollment relationship between students and courses.

5. **Input Handling:**
   - Handles user input for names, roll numbers, course codes, course names, and credits.
   - Incorporates input validation to ensure the correct data types are entered.

6. **Error Handling:**
   - Catches and prints `SQLExceptions` to handle database-related errors.

7. **Dynamic Data Entry:**
   - Allows the user to input details for multiple students, each with multiple courses.

8. **Data Display:**
   - After input, displays information about students and courses, providing an overview of the enrolled students and their courses.

This student management system is a console-based application that provides a basic framework for managing student information and their course enrollments in a database. Keep in mind that for the code to work properly, you need a MySQL database with the appropriate schema and tables, as mentioned in the code comments.
