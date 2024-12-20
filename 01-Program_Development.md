# Analysis

## Purpose of Analysis

The Analysis stage is the first step in program development. Its purpose is to:

- **Understand the problem**: Figure out what needs to be solved.
- **Identify requirements**: Determine what the program must do.

---

## Key Processes in Analysis

### 1. Abstraction

This means focusing on the important details and ignoring anything unnecessary. 

**Example**:  
Imagine you’re drawing a map of your school to show someone how to get to your classroom. You don’t draw every tree, chair, or bin—you only include the buildings, paths, and classroom numbers that are important for navigation.

---

### 2. Decomposition

This involves breaking a large problem into smaller, manageable parts.

**Example**:  
To break down the problem of drawing the map, start by identifying the smaller tasks that need to be completed:

- **Task 1**: Outline the entire school layout.
- **Task 2**: Highlight the buildings.
- **Task 3**: Mark the paths that connect buildings.
- **Task 4**: Add classroom numbers relevant to the route.
- **Task 5**: Remove unnecessary details like trees or bins.

  
<div align="center">
 
  ![School Map](https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/schoolmap.png)

</div>


# Design

## Purpose of Design

The Design stage plans how the program will work. By the end of this stage, the programmer knows:

- **What tasks the program will perform.**
- **How each task will work.**
- **How tasks will interact with each other.**

---

## Tools Used in Design

### 1. Flowcharts

These are diagrams that show the steps of a process.

**Example**:  
A flowchart for logging into a system might include:  
- Input username and password.  
- Check if they match the database.  
- Grant or deny access.

---

### 2. Structure Charts

These show how the program is divided into smaller modules.

**Example**:  
A shopping app might have modules like:  
- **Search Products**  
- **Add to Cart**  
- **Checkout**

---

### 3. Pseudocode

This is a way of writing the program's logic in simple, step-by-step language.

**Example**:  
A pseudocode for adding two numbers might look like this:

```text
INPUT number1
INPUT number2
SUM = number1 + number2
OUTPUT SUM
``` 
# Coding

## Purpose of Coding

In the Coding stage, the programmer writes the actual code using a programming language (e.g., Python, Java). This stage turns the design into a working program.

---

## Steps in Coding

1. **Write code for each module based on the design plan.**  
2. **Test the code for errors as you go (debugging).**  
3. **Combine modules to create the complete program.**

---

## Example

For a calculator program, the code for addition might look like this in Python:  

```python
# Addition module in Python
def add_numbers(a, b):
    return a + b

# Example usage
number1 = float(input("Enter the first number: "))
number2 = float(input("Enter the second number: "))
result = add_numbers(number1, number2)
print(f"The sum is: {result}")
````
 
# Testing

## Purpose of Testing

The Testing stage ensures that the program works correctly. A common method used is **Iterative Testing**.

---

## What is Iterative Testing?

1. **Test each module**: Check if it works as expected.  
2. **Fix errors (bugs)**: Correct any issues found.  
3. **Retest**: Repeat the process to confirm the error is fixed.  
4. **Combine and test modules**: Ensure they work together as a complete program.

---

## Example

**Testing a login module:**  

1. **Input valid credentials**: Ensure it grants access.  
2. **Input invalid credentials**: Ensure it denies access.  
3. **Fix issues**: If it behaves incorrectly, debug and retest.

