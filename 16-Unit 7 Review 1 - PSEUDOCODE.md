# Student Marks Analysis Algorithm

This algorithm calculates the highest, lowest, and average marks for four subjects (Maths, Science, English, and IT) across 600 students. It also provides overall statistics for all subjects combined.

## Question 1  
### A school with 600 students wants to produce some information from the results of the four standard tests in Maths, Science, English and IT. Each test is out of 100 marks. The information output should be the highest, lowest and average mark for each test and the highest, lowest and average mark overall. All the marks need to be input. 
a. Use pseudocode to write the algorithm to complete this task.

## Question 1 Breakdown

```pseudocode
// Initialisation of overall counters
OverallHighest ← 0
OverallLowest ← 100
OverallTotal ← 0
```
**Explanation:**
- **OverallHighest**: Stores the highest mark across all subjects and students, initialised to 0 (the lowest possible).
- **OverallLowest**: Stores the lowest mark across all subjects and students, initialised to 100 (the highest possible).
- **OverallTotal**: Accumulates the total sum of all marks to calculate the overall average later.

```pseudocode
FOR Test ← 1 TO 4 // Outer loop for each subject
```
**Explanation:**
- This loop iterates through the 4 subjects.
- **Test** represents the current subject (1 = Maths, 2 = Science, 3 = English, 4 = IT).

```pseudocode
    // Initialisation of subject counters
    SubjectHighest ← 0
    SubjectLowest ← 100
    SubjectTotal ← 0
```
**Explanation:**
- **SubjectHighest**: Tracks the highest mark for the current subject.
- **SubjectLowest**: Tracks the lowest mark for the current subject.
- **SubjectTotal**: Accumulates the total sum of marks for the current subject to calculate its average.

```pseudocode
    CASE OF Test
        1 : SubjectName ← 'Maths'
        2 : SubjectName ← 'Science'
        3 : SubjectName ← 'English'
        4 : SubjectName ← 'IT'
    ENDCASE
```
**Explanation:**
- This block assigns the correct **SubjectName** based on the current value of **Test**.

```pseudocode
    FOR StudentNumber ← 1 TO 600 // Inner loop for the students
```
**Explanation:**
- This loop iterates through all 600 students for the current subject.
- **StudentNumber** represents the student's position (1 through 600).

```pseudocode
        REPEAT
            OUTPUT 'Enter Student', StudentNumber, "'s mark for", SubjectName
            INPUT Mark
        UNTIL Mark >= 0 AND Mark <= 100 // Validate the mark range
```
**Explanation:**
- **OUTPUT** prompts the user to enter a mark for the current student and subject.
- **INPUT** reads the mark entered by the user.
- **REPEAT...UNTIL** ensures the mark is valid (between 0 and 100) before proceeding.

```pseudocode
        // Update subject-level statistics
        IF Mark < SubjectLowest THEN SubjectLowest ← Mark
        IF Mark > SubjectHighest THEN SubjectHighest ← Mark
        SubjectTotal ← SubjectTotal + Mark
```
**Explanation:**
- **SubjectLowest** is updated if the current mark is the lowest so far.
- **SubjectHighest** is updated if the current mark is the highest so far.
- **SubjectTotal** accumulates the marks for calculating the subject average.

```pseudocode
        // Update overall-level statistics
        IF Mark < OverallLowest THEN OverallLowest ← Mark
        IF Mark > OverallHighest THEN OverallHighest ← Mark
        OverallTotal ← OverallTotal + Mark
```
**Explanation:**
- **OverallLowest** is updated if the current mark is the lowest across all subjects and students.
- **OverallHighest** is updated if the current mark is the highest across all subjects and students.
- **OverallTotal** adds the mark to the overall total for calculating the overall average.

```pseudocode
    NEXT StudentNumber
```
**Explanation:**
- Moves to the next student in the loop.

```pseudocode
    // Calculate and display subject-level results
    SubjectAverage ← SubjectTotal / 600
    OUTPUT SubjectName
    OUTPUT "Average mark is ", SubjectAverage
    OUTPUT "Highest Mark is ", SubjectHighest
    OUTPUT "Lowest mark is ", SubjectLowest
```
**Explanation:**
- **SubjectAverage** calculates the average mark for the current subject by dividing **SubjectTotal** by 600.
- Outputs the subject's name, average mark, highest mark, and lowest mark.

```pseudocode
NEXT Test
```
**Explanation:**
- Moves to the next subject in the loop.

```pseudocode
// Calculate and display overall results
OverallAverage ← OverallTotal / 2400
OUTPUT "Overall Average is ", OverallAverage
OUTPUT "Overall Highest Mark is ", OverallHighest
OUTPUT "Overall Lowest Mark is ", OverallLowest
```
**Explanation:**
- **OverallAverage** calculates the average across all subjects by dividing **OverallTotal** by 2400 (600 students × 4 subjects).
- Outputs the overall average, highest mark, and lowest mark across all subjects.

---

## Summary
- The algorithm processes 600 students' marks in four subjects.
- It ensures data validity through input checks.
- It calculates and displays:
  - Subject-wise highest, lowest, and average marks.
  - Overall highest, lowest, and average marks across all subjects.

[Use this pseudocode compiler online.](https://pseudocode.deepjain.com/)

