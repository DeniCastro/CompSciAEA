# Maximum, minimum and average  
  
Finding the largest and smallest values in a list are two stndard methods that are frequently found in algorithms, for example, finding the highest and lowest mark awarded to a class of students.

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Maximum%2C%20minimum%20and%20average.jpg" alt="maximum, minimum and average" width="850"> 
</div>    

MaximumMark is set to 0. This assumes that no student will have a mark lower than 0.  
MinimumMark is set to 100. This assumes that no student will score more than 100.  
We start with extreme values and update them when we find a real student mark that is higher or lower.    

```FOR Counter ← 1 TO ClassSize```  

This means repeat the following steps for each student in the class.
Counter starts at 1 (representing the first student) and goes up to ClassSize (total number of students).
  
  ``IF StudentMark[Counter] > MaximumMark
    THEN
        MaximumMark ← StudentMark[Counter]
ENDIF
 ``    
 
  📌 What does this do?  

It checks if the current student’s mark is higher than the stored MaximumMark.  
If it is, then MaximumMark is updated to that student’s mark.  
👉 Example:  
If we have these marks: [55, 78, 90, 82]  
  
Start: MaximumMark = 0  
Compare: 55 > 0 → Yes, so MaximumMark = 55  
Compare: 78 > 55 → Yes, so MaximumMark = 78  
Compare: 90 > 78 → Yes, so MaximumMark = 90  
Compare: 82 > 90 → No, so MaximumMark stays 90  
At the end, the highest mark found is 90.  
  
``IF StudentMark[Counter] < MinimumMark
    THEN
        MinimumMark ← StudentMark[Counter]
ENDIF
``  
📌 What does this do?

It checks if the current student’s mark is lower than MinimumMark.
If it is, then MinimumMark is updated.
👉 Example:
If the marks are [55, 78, 90, 82], starting with MinimumMark = 100:

Compare: 55 < 100 → Yes, so MinimumMark = 55
Compare: 78 < 55 → No, so MinimumMark stays 55
Compare: 90 < 55 → No
Compare: 82 < 55 → No
At the end, the lowest mark found is 55.

``NEXT Counter
``
This tells the loop to move to the next student and repeat the process.  
Key Takeaways  

- Finding the Maximum (Highest) Mark

- Start with MaximumMark = 0.
- Compare each student’s mark to MaximumMark and update it if the student’s mark is higher.
- Finding the Minimum (Lowest) Mark

- Start with MinimumMark = 100.
- Compare each student’s mark to MinimumMark and update it if the student’s mark is lower.
- Looping through all students

- The FOR loop ensures each student’s mark is checked.

- If the largest and smallest values are not known, an alternative method is to set the maximum and minimum values to the first item in the list.    

For example, using this method to find the highest and lowest mark awarded to a class of students.  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Maximum%2C%20minimum%20and%20average2.jpg" alt="Maximum, minimum and average 2" width="850"> 
</div>
  
Calculating the average (mean) of all the values in a list is an extension of the totalling method, for example, calculating the average mark for a class of students.
  
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Maximum%2C%20minimum%20and%20average3.jpg" alt="Maximum, Minimum and average" width="850"> 
</div>
  
