# CourseGrader---cpp
Student Assignment and Grade Management.
## CourseGrader is a powerful WPF-based desktop application designed to streamline the management of student assignments and grades. This application enables educators to efficiently import, view, edit, and save student grades for various courses. The application reads data from Excel files and saves all course-related information in JSON format for persistent storage, ensuring that the original Excel files remain unaltered.
![image](https://github.com/user-attachments/assets/0cb1da12-89b3-46c6-9982-8fff2786b1dd)
![image](https://github.com/user-attachments/assets/263cb703-5b31-40fe-af58-e6fa6a2565ca)


## Key Features
- **File Importing**: Easily load an Excel file containing assignment grades. The file path is displayed in the application, and the course name (derived from the file name) is automatically set as the window title.
  
- **Course Management**: 
  - After importing a file, the course name is added to a ComboBox, with the course automatically selected.
  - The average of all final grades for the course is calculated and displayed.
  - A list of students enrolled in the course is displayed, sorted alphabetically by first name.

- **Student Data Management**:
  - Clicking on a student in the list displays their detailed information and grades for each assignment.
  - Grades can be edited directly within the application, with changes immediately reflected in the student's final grade.
  - A "Save" button allows for manual saving of updated grades to the course's JSON file.

- **Persistent Storage**: 
  - All course data is saved as JSON files named after the original Excel file, with a timestamp indicating the last update.
  - On startup, previously saved courses are loaded, allowing users to continue managing courses from where they left off.

- **Grade Adjustment**: 
  - A dedicated button opens a new window where users can select an assignment and apply a grade factor to all students in the course.

- **Data Storage**:
  - **JSON Files**: Used to store course and student data in a structured, easily accessible format.
  - **Excel Interop/EPPlus**: For reading data from Excel files.
