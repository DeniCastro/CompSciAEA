Python Basics: Practice

## 1. Introduction to Python: Running Your First Code
**Description:**  
Python is a **high-level, interpreted programming language**. You can run Python code using a compiler or an interactive shell.

**Question:**  
Edit the following code in a Python compiler by adding any message. What does it print?  
```python
print("!")
```

---

## 2. Understanding Errors in Python
**Description:**  
Errors occur when Python **doesn’t understand the code**. One common error is `SyntaxError`, which happens when the code structure is incorrect.

**Question:**  
Try running the following code and check the error message. Then, fix the error.
```python
print("Hello, world!"
```
**Hint:** Check for missing symbols.

---

## 3. Variables and Data Types
**Description:**  
A **variable** is a **named storage location** in Python. You don’t need to specify a type because Python automatically detects it.

**Question:**  
Run the following code and observe the output. What data type does Python assign to each variable?
```python
name = "Alice"
age = 25
height = 1.65
is_student = True

print(type(name))
print(type(age))
print(type(height))
print(type(is_student))
```

---

## 4. Constants in Python
**Description:**  
A **constant** is a value that **should not change** during the program's execution. Python does not have built-in constants, but by convention, we use **uppercase names** for constants.

**Question:**  
What will this code output?
```python
PI = 3.14159
radius = 5
circumference = 2 * PI * radius

print("The circumference is:", circumference)
```
**Bonus:** Change the value of `PI` and observe what happens.

---

## 5. Arithmetic Operations
**Description:**  
Python supports basic mathematical operations:  
- `+` (Addition)  
- `-` (Subtraction)  
- `*` (Multiplication)  
- `/` (Division)  
- `//` (Integer Division)  
- `%` (Modulus - remainder of division)  

**Question:**  
What will be the result of these calculations?
```python
a = 10
b = 3
print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
```

---

## 6. Understanding an Assignment Error
**Description:**  
In Python, `=` is used for **assigning values** to variables, while `==` is used for **comparison**. Misusing them can cause errors.

**Question:**  
Try running this code. What error appears? How can you fix it?
```python
x == 5
print(x)
```

---

## 7. String Manipulation
**Description:**  
Strings are **text data** enclosed in quotes. Python allows **concatenation (joining)** and **repetition** of strings.

**Question:**  
What will this code print?
```python
greeting = "Hello"
name = "Alice"
message = greeting + ", " + name + "!"
print(message)

repeat = "Python " * 3
print(repeat)
```
**Bonus:** What happens if you try `message - name`?

---

## 8. Fixing an Error with Strings and Numbers
**Description:**  
Python **does not allow** direct operations between strings and numbers.

**Question:**  
Try running this code. What error do you get? Fix it.
```python
age = 25
print("I am " + age + " years old.")
```

---

## 9. Reading and Writing to a File
**Description:**  
Python can **store and retrieve data** using files. The `open()` function allows reading (`"r"`) and writing (`"w"`).

**Question:**  
Complete the missing part of the code to **write** `"Hello, Python!"` into `example.txt`, then read and print it.
```python
# Write to file
with open("example.txt", "w") as file:
    file.______ ("Hello, Python!")  # Fill in the missing part

# Read from file
with open("example.txt", "r") as file:
    content = file.read()

print(content)
```
**Bonus:** What happens if you change `"w"` to `"a"`?

---

## 10. Debugging a Simple Error
**Description:**  
A `NameError` occurs when Python **cannot find** a variable that is being used.

**Question:**  
Try running this code. Identify the error and fix it.
```python
print(favorite_color)
favorite_color = "blue"
```

---
