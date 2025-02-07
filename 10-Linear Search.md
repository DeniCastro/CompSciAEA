# 7.4.4 Linear Search  
# Linear Search in Computer Science

## What is a Search?
A **search** is used to check if a value is stored in a list by systematically working through the items in the list. There are different search methods, but for IGCSE Computer Science, you only need to understand **linear search**.

## What is a Linear Search?
A **linear search** inspects each item in a list one by one until it finds the value being searched for or reaches the end of the list.


A search is used to check if a value is stored in a list, performed systematically working through the items in the list. There are several standaard search methods, but you only need to understand one method for IGCSE Computer Science. This is called a **linear search**, which inspects each item in a list in turn to see if the item matches the value searched for.    

### Example Scenario
Imagine you are searching for a name in a class list of student names, where all the names stored are different. The search should check each name in the list until it finds the one you are looking for.


<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Linear%20Search%201.jpg" alt="Linear Search 1" width="800"> 
</div>    


<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Linear%20Search%202.jpg" alt="Linear Search 2" width="800"> 
</div>      

  
## Pseudocode for Linear Search
```plaintext
OUTPUT "Please enter name to find"
INPUT Name
Found ← False
Counter ← 1
REPEAT
    IF Name = StudentName[Counter] THEN
        Found ← TRUE
    ELSE
        Counter ← Counter + 1
    ENDIF
UNTIL Found OR Counter > ClassSize

IF Found THEN
    OUTPUT Name, "Found at position", Counter, "in the list."
ELSE
    OUTPUT Name, "Not Found."
ENDIF
```

### How Does the Algorithm Work?
1. The user is asked to enter a name to search for.
2. The variable **Found** is initially set to `False`.
3. A **Counter** is initialized at `1` (assuming lists start at index 1 in this pseudocode).
4. A **REPEAT UNTIL** loop is used to keep searching:
   - If the current **StudentName[Counter]** matches the **Name** being searched for, it updates `Found` to `True`.
   - Otherwise, it moves to the next student in the list by increasing **Counter**.
   - The loop stops if the name is found or if all names in the list have been checked.
5. After exiting the loop:
   - If `Found` is `True`, the program outputs the name and its position in the list.
   - Otherwise, it displays that the name was **not found**.

## Python Implementation
Here's how we can write this search algorithm in Python:
```python
# Get user input
name_to_find = input("Please enter name to find: ")

# Sample list of student names
student_names = ["Alice", "Bob", "Charlie", "David", "Eve"]

# Initialize variables
found = False
counter = 0  # Lists in Python start at index 0

# Linear search loop
while not found and counter < len(student_names):
    if student_names[counter] == name_to_find:
        found = True
    else:
        counter += 1

# Display result
if found:
    print(f"{name_to_find} found at position {counter + 1} in the list.")
else:
    print(f"{name_to_find} not found.")
```

## Key Takeaways
- **Linear search** checks each item one by one.
- It is simple but can be slow for large lists.
- It stops as soon as the item is found or after checking all elements.
- Python lists start at index **0**, so we adjust the position when displaying results.

This method is useful for small lists and when searching for a value without knowing its exact position in advance. 🚀

# Counting Occurrences in a List

## Introduction
This method is useful for small lists and when searching for a value without knowing its exact position in advance. Instead of just checking whether a value exists in a list, we count how many times it appears.

For example, if we want to find how many students in a class have chosen "ice cream" as their favourite dessert, we can use a loop to count each occurrence.

---

## Pseudocode
```plaintext
ChoiceCount ← 0
FOR Counter ← 1 TO Length
    IF "ice cream" = Dessert[Counter] THEN
        ChoiceCount ← ChoiceCount + 1
NEXT Counter
OUTPUT ChoiceCount, "chose ice cream as their favorite dessert."
```

### Explanation of Pseudocode
1. **Initialize the counter:** We start by setting `ChoiceCount` to 0. This variable will store the number of times "ice cream" appears in the list.
2. **Loop through the list:** We iterate through all elements of the `Dessert` list using a `FOR` loop.
3. **Check for a match:** Inside the loop, we check if the current dessert choice is "ice cream".
4. **Increase the counter:** If a match is found, we increase `ChoiceCount` by 1.
5. **Output the result:** After the loop finishes, we display how many times "ice cream" was chosen.

---

## Converting Pseudocode to Python
Below is how we can implement this algorithm in Python:

```python
# List of dessert choices
Dessert = ["cake", "ice cream", "pie", "ice cream", "cookies", "ice cream"]

# Initialize counter
ChoiceCount = 0

# Loop through each dessert choice
for dessert in Dessert:
    if dessert == "ice cream":
        ChoiceCount += 1

# Output result
print(ChoiceCount, "chose ice cream as their favorite dessert.")
```

### Explanation of Python Code
1. We define a list `Dessert` containing different dessert choices.
2. We initialize `ChoiceCount` to 0.
3. We use a `for` loop to go through each item in `Dessert`.
4. If the current dessert is "ice cream", we increase `ChoiceCount` by 1.
5. Finally, we print the result.

---

## Summary
- This method is helpful for counting occurrences of an item in a list.
- We use a loop to check each item and update a counter variable.
- The concept applies to many real-world problems, such as counting votes or tracking responses in surveys.

Now, try modifying the list to count other dessert choices! 🍨🎂🍪



<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Linear%20Search%203.jpg" alt="Linear Search 3" width="800"> 
</div>  
  
## 7.4.5 Bubble sort  
Lists can be more useful if the items are sorted in a meaningful order. For example, name could be sorted in alphabetical order, or temperatures could be sorted in ascending or descending order. There are several standard sorting methods available, but you only need to understand one method for IGCSE Computer Science.  
This method of sorting is called **bubble sort**. Each element is compared with next element and swapped if the elements are in the wrong order, starting from the first element and finishing with the next-to-last element. Once it reaches the end of the list, we can be sure that the last element is now in the correct place. However, other items in the list may still be out of order. Each element in the list is compared again apart from the last one because we know the final element is in the correct place. This continues to repeat until there is only one element to check or no swaps are made.
  
  
For example, the bubble sort algorithm can be used to sort a list of ten temperatures stored in the array, **Temperature[]**, into ascending order. It could be written in pseudocode as:  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Bubble%20sort.jpg" alt="Bubble sort" width="800"> 
</div>  

