# -FILE-HANDLING-PROGRAM
*COMPANY*: CODTECH IT SOLUTIONS PVT.LTD
**NAME*: DILIP KUMAR MURMU
*INTERN ID*: CT04DF2445
*DOMAIN*: C LANGUAGE
*DURATION*: 4 WEEKS
*MENTOR*: NEELA SANTOSH KUMAR

#Task 1 Description – File Handling Program in C

The objective of Task 1 is to create a C program that demonstrates the implementation of file handling operations, including creating, writing to, reading from, and appending data to files. This task is an essential introduction to persistent data storage techniques in the C programming language, forming a base for building larger and more complex systems such as record management systems, logs, and data processors.

In C, file handling is managed through the standard input/output library <stdio.h>, which provides powerful functions for interacting with files on the system. This program introduces users to key file operations and allows them to practice working with file pointers (FILE *), file modes, and common I/O functions like fopen(), fprintf(), fgetc(), fputs(), and fclose().

The program begins by defining a main() function that offers the user a menu-driven interface with four options:
1. Create and Write to File
2. Append to File
3. Read from File
4. Exit

This looping menu ensures that the user can perform multiple operations in a single session, giving them flexibility to test how file contents change with each operation.

At the core of this program are three custom-defined functions:

1. writeFile(const char* filename)


2. appendFile(const char* filename)


3. readFile(const char* filename)
..........
1. writeFile()

This function opens the file in write mode ("w"). If the specified file already exists, its content is erased and replaced with new input. If the file does not exist, it is automatically created. The user is prompted to enter a string of data, which is captured using fgets() to support multi-word input. The data is then written into the file using fputs(), and the file is closed using fclose() to ensure proper saving of data. This function is ideal for situations where fresh data needs to be saved, such as writing configuration files or creating new documents.


2. appendFile()

The appendFile() function is used to add data to the end of an existing file without removing the previous content. It opens the file in append mode ("a"), allowing the user to add more lines or entries. This operation is essential in scenarios such as logging, where existing content must be preserved, and new information added continuously. The use of fputs() ensures simple and direct insertion of text at the end.

3. readFile()

The readFile() function allows the user to view the contents of the file by opening it in read mode ("r"). It reads characters one at a time using fgetc() until the end-of-file (EOF) is reached. The contents are displayed on the console, giving the user real-time feedback on what is stored in the file. This operation is critical in many real-world applications, such as reading saved data, displaying reports, or verifying file contents.

Additional Features and Highlights

The program includes input validation to ensure the user selects only the available menu options.

File creation is handled securely using fopen() and error-checking to detect if the file could not be created or accessed.

The use of fclose() after every file operation demonstrates best practices in resource management, helping avoid memory or file descriptor leaks.


Real-World Applications

This file handling task is not just an academic exercise; it directly maps to several real-world use cases:

Building student record systems

Implementing log and audit trail generators

Creating note-taking applications

Reading/writing configuration and settings files

Storing data for later analysis

#OUTPUT: 
![Image](https://github.com/user-attachments/assets/4b3d95b7-2ded-41f8-bb62-2f8cd78a01df)


