# CASE OF... OTHERWISE... ENDCASE  
For a **CASE** statement the value of a variable decides the path to be taken.  
Several values are usually specified. **OTHERWISE** is the path taken for all other values. The end of the statement is shown by **ENDCASE**.  

Have a look at the algorithm below that specifies what happens if the value of **Choice** is **1**, **2**, **3** or **4**.  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/CASE%20OF%20Choice.jpg" alt="CASE OF Choice" width="500"> 
</div>
  
## The pseudocode for iteration  
When some actions performed as part of an algorithm need repeating this is called iteration. Loop structures are used to perform the iteration.  
Pseudocode includes these three different types of loop structure:  

A set of number of repetitions **FOR ... TO ... NEXT**  
A repetition, where the number of repeats is not known, that is completed at least once: **REPEAT ... UNTIL**  
A repetition, where the number of repeats is not known, that may never be completed: **WHILE ... DO ... ENDWHILE***  

All types of loops can all perform the same task, for example displaying ten stars:  
  
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/loop_structure.jpg" alt="CASE OF Choice" width="500"> 
</div>

## FOR ... TO... NEXT loops  
A variable is set up, with a start value and an end value, this variable is incremented in steps of one until the end value is reached and the iteration finishes. The variable can be used within the loop so long as its value is not changed. This type of loop is very useful for reading values into lists with a known length.    

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/for...to...next%20loops.jpg" alt="FOR ... TO... NEXT Loops" width="500"> 
</div>  

## REPEAT ... UNTIL loop  
This loop structure is used when the number of repetitions/iterations is not known and the actions are repeated **UNTIL*** a given condition becomes true. The actions in this loop are always completed at least once. This is a post-condition loop as the test for exiting the loop is at the end of the loop.  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/REPEAT...%20UNTIL...%20loop.jpg" alt="REPEAT ... UNTIL" width="500"> 
</div>    
  
## WHILE ... DO ... ENDWHILE loop  
This loop structure is used when the number of repetitions/iterations is not known and the action are only repeated **WHILE** a given condition is true. If the **WHILE** condition is untrue then the actions in this loop are never performed. This is a pre-condition loop as the test for exiting the loop is at the beginning of the loop.  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/WHILE...%20DO...%20ENDWHILE%20loop.jpg" alt="WHILE... DO... ENDWHILE loop" width="500"> 
</div>    


# Loops in Programming – Extended + Python

Loops are like magic spells in programming! 🧙✨ They help us repeat something over and over again without writing the same instructions multiple times.

Imagine you have to write “Hello!” 100 times. That would take a long time! Instead, we can use loops to tell the computer, **“Hey, repeat this for me!”**

There are three types of loops we’ll learn:

1. **For Loop** – When we know how many times to repeat.
2. **Repeat Until Loop** – When we repeat **until** something happens.
3. **While Loop** – When we keep repeating **as long as** something is true.

---

## 1️⃣ For Loop
A **For Loop** is used when we already know how many times we want to repeat something.

### **Pseudocode Example:**
```
FOR i FROM 1 TO 5 DO
    OUTPUT "Hello!"
NEXT i
```
### **How it works:**
1. Start with `i = 1`.
2. Print "Hello!".
3. Add 1 to `i`.
4. If `i` reaches 5, stop.

### **Python Code:**
```python
for i in range(1, 6):  # The loop repeats 5 times (1 to 5)
    print("Hello!")
```

---

## 2️⃣ Repeat Until Loop
A **Repeat Until Loop** repeats the action **until** a condition becomes true.

### **Pseudocode Example:**
```
REPEAT
    OUTPUT "Keep going!"
UNTIL user_input = "stop"
```
### **How it works:**
1. Print "Keep going!".
2. Ask the user for input.
3. If they type "stop", the loop ends.

### **Python Code:**
Python does not have `REPEAT UNTIL`, but we can use a `while` loop to do the same thing.
```python
user_input = ""
while user_input != "stop":  # Keep repeating until the user types "stop"
    print("Keep going!")
    user_input = input("Type 'stop' to end: ")
```

---

## 3️⃣ While Loop
A **While Loop** repeats **as long as** a condition is true.

### **Pseudocode Example:**
```
WHILE counter < 3 DO
    OUTPUT "Counting..."
    counter ← counter + 1
ENDWHILE
```
### **How it works:**
1. Start with `counter = 0`.
2. Print "Counting...".
3. Add 1 to `counter`.
4. If `counter` reaches 3, stop.

### **Python Code:**
```python
counter = 0
while counter < 3:
    print("Counting...")
    counter += 1  # Increase counter by 1
```

---

### 🔥 Summary
| Loop Type          | When to Use It | Example |
|-------------------|--------------|---------|
| **For Loop**     | When we know how many times to repeat | Counting from 1 to 10 |
| **Repeat Until** | When we stop when a condition is met | Asking for a password until it's correct |
| **While Loop**   | When we keep repeating while a condition is true | Counting down until a timer reaches 0 |

