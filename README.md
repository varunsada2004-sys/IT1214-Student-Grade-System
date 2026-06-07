Student Grading System
#Initial Project Setup
Project Purpose
​The Student Grade Management System is a console-based Java application developed to assist educational institutes in transitioning from manual record-keeping to a digital solution. It provides an efficient way to manage academic records by allowing teachers to:
​Add new student information (ID, Name, and Marks).
​View a comprehensive list of all stored student records.
​Search for specific students using their unique ID.
​Calculate and display the average academic performance of all students in the system.
​This project is developed using Object-Oriented Programming (OOP) principles to ensure data encapsulation and maintainable code structure.

How to Run: 
​To run this application, ensure you have the Java Development Kit (JDK) installed on your system.
Follow these steps:
  1) Download the Repository as ZIP file.
  2) Navigate to the directory in cmd
  3) Compile the GradeSystem.java using the command "javac GradeSystem.java".
  4) Run the Application using the command "java GradeSystem".

How it works:
1.The Data Structure (The Student Class)
​The Student class serves as a blueprint. Every time you add a student, you are creating an "instance" of this class. It encapsulates the data, meaning it bundles the ID, Name, and Marks together into one unit.
​The Constructor: When you type new Student(...), it initializes these values for that specific student.
​Getters: These methods allow the GradeSystem to "read" the data without being able to accidentally overwrite it (this is a core OOP concept).
​2. The Management System (GradeSystem.java)
​This is the "Brain" of your application. It controls the flow of information:
​Data Storage (ArrayList): We use private static ArrayList<Student> students. Think of this as a dynamic, digital shelf where we store each Student object. It automatically grows as you add more students.
​The Main Menu (while loop): The code enters an infinite loop (while (!exit)) that keeps the console open. It uses a switch statement to route your input to the correct method.
​Data Processing:
​      2.1)Adding: The code captures input via Scanner, creates a new Student object, and uses .add() to place it on our digital shelf.
​      2.2)Searching: The program uses a linear search (a for-each loop) to look at every student on the shelf one by one, comparing their ID to the ID you entered.
​      2.3)Calculation: It iterates through the ArrayList to sum up all marks, then divides by the list size to calculate the average.
​3. Execution Flow
​When you run the code, the Java Virtual Machine (JVM) performs these steps:
​Loading: It loads the GradeSystem class into memory.
​Initialization: It prepares the ArrayList to hold student data.
​Interaction: It waits for your input via Scanner.
​Transformation: It maps your menu choice (1, 2, 3, etc.) to the logic defined in your methods.
