# Assignment- 3 JAVA 
The program is a basic implementation of a student management system. It allows the user to insert, delete, update, search and display student records. The student record consists of PRN (Personal Registration Number), Name, Date of Birth (DOB), and marks.

The program defines a Student class that has PRN, Name, DOB, and marks as its member variables. It also defines a nested DOB class that represents a date of birth. The Student class has getter and setter methods for each member variable, and a calculateGrade() method that returns a string representing the grade calculated based on the student's total marks.

The StudentList class has an ArrayList to store the student records, and methods to perform the operations mentioned earlier. The processAdd(), processDelete(), processUpdate(), processSearch(), and processDisplay() methods implement the respective operations. The switchInput() method is responsible for selecting the appropriate operation based on the user's input.

The main method initializes an ArrayList of Student objects, a Scanner object, and a boolean flag indicating whether the list is sorted or not. It then enters a loop where it prompts the user to enter a number corresponding to the desired action, reads the input, and calls a corresponding method.

The switchInput method is used to handle each possible action based on the user's input. It uses a switch statement to call the appropriate method based on the user's input.

The program also defines a CompareByMarks class that implements the Comparator interface and compares two Student objects based on their total marks.

The processAdd method is called when the user wants to add a student to the list. It prompts the user to enter the student's PRN, name, date of birth, and marks. It then creates a new Student object using the entered values and adds it to the ArrayList, as long as a student with the same PRN doesn't already exist in the list.

The processDelete method is called when the user wants to delete a student from the list. It prompts the user to enter the PRN of the student to be deleted and searches the list for a student with that PRN. If a student is found, it is removed from the list.

The processUpdate method is called when the user wants to update a student's information. It prompts the user to enter the PRN of the student to be updated and searches the list for a student with that PRN. If a student is found, the user is prompted to enter the updated information, which is used to create a new Student object. The existing student's information is then updated with the new information, as long as the new information isn't blank or -1.

The processSearch method is called when the user wants to search for a student. It prompts the user to select a search method (by PRN, by name, or by index) and calls the corresponding search method. The search methods then return the found student or null if no student is found.

The processDisplay method is called when the user wants to display the list of students. If the list isn't sorted, it is sorted by the CompareByMarks comparator. The displayList method is then called, which prints out each student's information.

The Student class is an inner class of the StudentList class. It represents a student and contains fields for the student's PRN, name, date of birth, and marks. It also contains methods to get and set the fields, as well as a private method to calculate the student's grade based on their marks. The DOB class is another inner class that represents a date of birth and contains fields for the day, month, and year.

Overall, the program is a basic implementation of a student management system that allows the user to perform basic operations on student records.
