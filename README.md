# appointment_managementsystem_using_priorityqueue
The appointments for the patients are given priority wise based on the emergency of disease and the patient.
The patients neccesary details are taken.
Using PRIORITY QUEUE the appointments are alloted for each patient.
This Java code represents a simple appointment management system for a hospital called KIMS (Kohinoor Institute of Medical Sciences). The system allows users to add patients for doctor's appointments, delete patient records, and display the list of appointments.

The code starts with the definition of a `Node` class, which represents a single node in a linked list. Each node contains information about a patient, such as their name, age, address, phone number, blood group, registration number, and priority. The `Node` class has a reference to the next node in the linked list.

The `Main` class is the main entry point of the program. It contains the `main` method where the execution of the program begins. The program presents a menu-based user interface using a `do-while` loop, allowing users to choose different options:

1. **Add a patient for a doctor's appointment**: Users can enter the details of a patient, including their name, age, address, phone number, blood group, and choose a disease number as the priority for the appointment. The `insert` method is called to insert the patient's information into the linked list based on their priority.

2. **Delete a patient from the record**: If there are patients in the appointment list, this option allows the deletion of the first patient's record from the linked list. The `delete` method is called to remove the first node from the list.

3. **Display all appointments**: This option displays the details of all the patients in the appointment list. The `display` method is called to iterate through the linked list and print the information of each patient.

4. **Exit**: Terminates the program.

The `insert` method is responsible for adding a new patient to the linked list in a sorted manner based on their priority. The patient's details are obtained from user input, and a new `Node` object is created. The `getPriority` method prompts the user to enter a disease number to determine the priority of the appointment. The `insert` method then inserts the new node at the appropriate position in the linked list based on its priority.

The `delete` method removes the first node from the linked list if it exists. It updates the `start` reference to point to the next node and frees the memory occupied by the deleted node.

The `display` method iterates through the linked list starting from the `start` node and prints the details of each patient in a formatted manner. If the list is empty, it displays a message indicating no appointments for the day.

The `table` method prints a table of disease numbers and their corresponding diseases, which is used for displaying options to the user when selecting the priority for a patient's appointment.

The `clearScreen` method is responsible for clearing the console screen by printing special characters.

Overall, this code provides a basic framework for managing appointments at KIMS Hospital, allowing users to add, delete, and view appointments using a linked list data structure.
