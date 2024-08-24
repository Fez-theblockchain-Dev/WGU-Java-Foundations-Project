# WGU-Java-Foundations-Project
Final Capstone project for Western Governors University "Intro to Java" class

### 1.1 **Project Name**

Student Grade Calculator

### 1.2 **Project Summary**

The Student Grade Calculator is a console-based Java application designed to calculate the final grade for students based on their scores in different subjects. The program will allow users (teachers or students) to input scores for various subjects, calculate the average score, and determine the corresponding final grade (A, B, C, D, F) based on predefined grading criteria.
________________________________________________________________________________________________________________________________________

## 2. **Requirements**

- The application shall allow the user to input the student's name & input scores for a minimum of three and a maximum of six subjects, 
- Validate that the input scores are numerical and within the range of 0 to 100%.

### 2.1.2 **Grade Calculation**

- The application shall calculate the average score by summing all subject scores and dividing by the number of subjects.
- The application shall assign a final grade based on the following criteria:
    - A: 90 - 100
    - B: 80 - 89
    - C: 70 - 79
    - D: 60 - 69
    - F: 0 - 59

### **Output**

- application displays the student's name, the average score, and the corresponding final grade.
- Application handles and display appropriate messages for invalid inputs or errors (proper error handeling)

### 2.2 **Non-Functional Requirements**

### 2.2.1 **Usability**

- The application shall have a simple, text-based interface that is easy to use.
- The application shall provide clear instructions and error messages to guide the user.

### 2.2.2 **Performance**

- The application shall process input and display the results instantly.
- The application shall be optimized to handle typical classroom scenarios (e.g., processing grades for up to 30 students sequentially).

### 2.2.3 **Reliability**

- The application shall validate user input to minimize errors.
- The application shall not crash on invalid input but instead prompt the user to re-enter the data.

## 3. **Scope**

### 3.1 **In Scope**

- Basic input validation for scores.
- Calculation of the average score and final grade.
- Displaying results in the console.

### 3.2 **Out of Scope**

- Persistent data storage (e.g., saving grades to a file).
- Advanced user interfaces (e.g., graphical UI).
- Handling different grading scales (e.g., weighted grades, plus/minus grading).

## 4. **Assumptions**

- The user has basic knowledge of using a console application.
- All inputs are expected to be valid numeric values; any non-numeric input will prompt the user to re-enter the data.

## 5. **Dependencies**

- Java Development Kit (JDK) 17.
- IDE for Java development (e.g., IntelliJ IDEA, Eclipse).
- No external libraries or frameworks are required for this project.

## 6. **Project Milestones**

### 6.1 **Phase 1: Initial Setup (1 week)**

- Set up the development environment.
- Create the basic project structure.

### 6.2 **Phase 2: Core Functionality (2 weeks)**

- Implement user input for student names and scores.
- Implement the logic for calculating the average score and determining the final grade.

### 6.3 **Phase 3: Testing and Validation (1 week)**

- Perform unit testing to ensure all calculations are accurate.
- Test for edge cases, such as minimum and maximum score inputs.

### 6.4 **Phase 4: Final Review and Submission (1 week)**

- Conduct a final code review.
- Prepare documentation (e.g., user manual, code comments).
- Submit the project.

## 7. **Technical Design**

### 7.1 **Class Structure**

### 7.1.1 **Main Class: `StudentGradeCalculator`**

- **Purpose:** This class will contain the `main` method and will be responsible for the application's execution flow.
- **Responsibilities:**
    - Initialize the program.
    - Handle user input.
    - Call methods to calculate the average score and determine the final grade.
    - Display the results.

### 7.1.2 **Helper Class: `Student`**

- **Purpose:** This class will represent a student with attributes such as name and an array of scores.
- **Attributes:**
    - `String name`
    - `int[] scores`
- **Methods:**
    - `double calculateAverage()`: Calculates the average of the student's scores.
    - `char determineGrade(double average)`: Returns the final grade based on the average score.

### 7.2 **User Interaction Flow**

1. The program starts and prompts the user to enter the student's name.
2. The user is prompted to enter scores for each subject.
3. The program calculates the average score.
4. The program determines the final grade based on the average score.
5. The results are displayed to the user.

## 8. **Risks and Mitigation**

### 8.1 **Risk: Input Validation**

- **Description:** Users may input non-numeric values or scores outside the valid range.
- **Mitigation:** Implement robust input validation and error handling to prompt the user to re-enter data when invalid input is detected.

### 8.2 **Risk: Calculation Errors**

- **Description:** Errors in calculating the average score or determining the grade could lead to incorrect results.
- **Mitigation:** Use unit testing to validate all calculations and handle edge cases.

## 9. **Conclusion**

The Student Grade Calculator is a simple yet effective tool for calculating and displaying student grades based on their academic performance. This project will demonstrate a solid understanding of Java basics, including input handling, conditional logic, loops, and object-oriented programming.
