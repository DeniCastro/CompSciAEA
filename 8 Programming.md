# Programming 

<div align="center">
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/Programming/img/programming-title.jpg" alt="Programming Title" width="500">
</div>   

## Concepts

So far, you have tested your algorithms by dry-running. Once you have written a program for your algorithm, and when there are no syntax errors, you will now use a computer to run the program to complete the task exactly as you have written it; you may need to make some changes before it works exactly as you intend it to.

This chapter will introduce you to the programming concepts required for practical use of a high-level language. This chapter shows the concepts behind such programming languages but should be used in conjunction with learning the syntax of an appropriate programming language.

There are many high-level programming languages to choose from. For IGCSE Computer Science, the high-level programming languages recommended are **Python**, **Visual Basic**, or **Java**. The use of these languages is also required for A Level Computer Science.

Many programming languages need an **Integrated Development Environment (IDE)** to write and run code. IDEs are free to download and use.

---

### Python will be the primary programming language used in this IGCSE course because:
- **Easy to Learn**: Python has a simple and readable syntax, making it ideal for beginners.
- **Versatile**: It is used in various fields, including web development, data analysis, artificial intelligence, and more.
- **Wide Community Support**: Python has a large community, so finding help and resources is easy.
- **Free and Open Source**: Python is free to use and distribute.

---
# Python Programming for IGCSE

## Introduction

In this IGCSE Computer Science course, we will use **Python** as our programming language. Python is a popular, beginner-friendly language known for its simplicity and readability. Throughout this course, you will learn how to write and understand Python code to solve problems and complete tasks.

## Data Types in Python

In Python, data types refer to the kind of value a variable can hold. Here are some of the basic data types we will work with:

### 1. Integer (int)
Integers are whole numbers (positive or negative) without decimals.

**Example:**
```python
# Integer example
number = 10
print(number)  # Output: 10
```

### 2. Float (float)
Floats are numbers with decimal points.

**Example:**
```python
# Float example
pi = 3.14
print(pi)  # Output: 3.14
```

### 3. String (str)
Strings are sequences of characters (letters, numbers, symbols) enclosed in quotes.

**Example:**
```python
# String example
name = "Alice"
print(name)  # Output: Alice
```

### 4. Boolean (bool)
Booleans represent **True** or **False** values. They are useful for decision-making.

**Example:**
```python
# Boolean example
is_python_fun = True
print(is_python_fun)  # Output: True
```

### 5. List (list)
Lists store multiple items in a single variable. Items in a list are ordered and can be changed.

**Example:**
```python
# List example
fruits = ["apple", "banana", "cherry"]
print(fruits)  # Output: ['apple', 'banana', 'cherry']
```

### 6. Tuple (tuple)
Tuples are like lists but **cannot** be changed (they are immutable).

**Example:**
```python
# Tuple example
coordinates = (10, 20)
print(coordinates)  # Output: (10, 20)
```

### 7. Dictionary (dict)
Dictionaries store data in **key-value** pairs.

**Example:**
```python
# Dictionary example
student = {"name": "Alice", "age": 16}
print(student)  # Output: {'name': 'Alice', 'age': 16}
```

# Python Lists and Dictionaries

## 📋 Lists

A **list** is an ordered collection of items. You can store multiple values in a single variable using a list.

### 🔹 Creating a List

```python
subjects = ["Maths", "English", "Science"]
```

### 🔹 Accessing Items

```python
print(subjects[0])  # Outputs: Maths
print(subjects[2])  # Outputs: Science
```

### 🔹 Adding Items to a List

```python
subjects.append("History")
print(subjects)  # Outputs: ['Maths', 'English', 'Science', 'History']
```

### 🔹 Looping Through a List

```python
for subject in subjects:
    print(subject)
```

### 🔹 Using Inputs with Lists

```python
marks = []
for i in range(5):
    mark = float(input(f"Enter mark {i+1}: "))
    marks.append(mark)

print("You entered:", marks)
```

---

## 📘 Dictionaries

A **dictionary** stores data in key-value pairs. It’s useful when you want to label each value.

### 🔹 Creating a Dictionary

```python
grades = {
    "Maths": 85,
    "English": 78,
    "Science": 92
}
```

### 🔹 Accessing Items

```python
print(grades["Maths"])  # Outputs: 85
```

### 🔹 Adding/Updating Items

```python
grades["History"] = 88  # Add new key-value pair
grades["Maths"] = 90    # Update existing value
```

### 🔹 Looping Through a Dictionary

```python
for subject, grade in grades.items():
    print(f"{subject}: {grade}")
```

### 🔹 Using Inputs with Dictionaries

```python
subjects = ["Maths", "English", "Science"]
grades = {}

for subject in subjects:
    grade = float(input(f"Enter your grade for {subject}: "))
    grades[subject] = grade

print(grades)
```

---

## ✅ Summary

| Structure   | Mutable | Ordered | Syntax         | Example Usage              |
|-------------|---------|---------|----------------|----------------------------|
| List        | Yes     | Yes     | `[]`           | Store marks or names       |
| Dictionary  | Yes     | No      | `{key: value}` | Store subject:grade pairs  |




