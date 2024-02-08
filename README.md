Project Overview
The University Exam Scheduler is a Java-based application designed to automate the process of scheduling exams for a university. It handles various constraints such as exam conflicts, professor availability, and classroom capacities. The program reads data from CSV files, creates a graph-based representation of exams, and utilizes algorithms to efficiently schedule exams with minimal student conflicts.

Features
Exam Conflict Resolution: Detects and resolves exam scheduling conflicts.
Block Course Handling: Manages block courses with pre-defined schedules.
Dynamic Classroom Assignment: Assigns classrooms based on student count and availability.
Simulated Annealing Algorithm: Optimizes scheduling to reduce student exam conflicts.
Flexible Timetabling: Supports a 6-day schedule with an option to extend to Sunday if needed.

File Structure
ClassList.java: Manages class lists including student IDs, professor names, course IDs, and exam durations.
Classroom.java: Represents classrooms with attributes like room ID and capacity.
Exam.java: Core class for handling exam details, conflicts, and scheduling.
AllExam.java: Holds a collection of all exams and manages relationships between them.
Main.java: The main driver program that ties together all components.

Input Files
1000student.csv : Contains student-related data for exams.
Classes.csv           : Lists available classrooms and their capacities.
classlist.csv ,example.csv : They are csv files that contains the IDs of all students and then information about the exam of the course they took (professor teaching the course, course code and exam duration).
Setup and Execution
Prerequisites: Ensure Java is installed on your system.
Compiling: Use javac to compile all .java files. Example: javac Main.java.
Running the Application: Execute the main class using java Main.
CSV File Paths: Modify the file paths in Main.java if the CSV files are located in a different directory.

Usage Guide
Reading CSV Files: The program reads classroom and student data from CSV files at startup.
Block Course Input: Users are prompted to enter block course details interactively.
Exam Scheduling: The program automatically schedules exams, considering various constraints.
Output: Scheduled exams with room assignments are displayed, along with a fault score indicating the number of student conflicts.
