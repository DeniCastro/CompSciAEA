## **Understanding f-strings in Python**  

### **What are f-strings?**  
In Python, **f-strings** (formatted string literals) provide a simple way to format strings dynamically. They allow you to insert variables, expressions, and even functions inside curly braces `{}` within a string.  

f-strings were introduced in **Python 3.6** and are prefixed with the letter `f` (or `F`) before the opening quotation mark.

---

### **Basic Syntax**  
```python
name = "Alice"
age = 25
print(f"My name is {name} and I am {age} years old.")
```
**Output:**  
```
My name is Alice and I am 25 years old.
```

---

### **Using Expressions in f-strings**  
You can perform calculations and even call functions inside f-strings.  
```python
num1 = 10
num2 = 5
print(f"The sum of {num1} and {num2} is {num1 + num2}.")
```
**Output:**  
```
The sum of 10 and 5 is 15.
```

---

### **Formatting Numbers**  
f-strings allow you to format numbers with specific decimal places.  
```python
pi = 3.1415926535
print(f"Pi rounded to 2 decimal places: {pi:.2f}")
```
**Output:**  
```
Pi rounded to 2 decimal places: 3.14
```

---

### **Using f-strings with Dictionaries and Lists**  
You can access elements inside lists and dictionaries easily.  
```python
student = {"name": "John", "grade": "A"}
print(f"Student: {student['name']}, Grade: {student['grade']}")

fruits = ["Apple", "Banana", "Cherry"]
print(f"My favorite fruit is {fruits[1]}.")
```
**Output:**  
```
Student: John, Grade: A
My favorite fruit is Banana.
```

---

### **Using f-strings with Functions**  
```python
def square(num):
    return num * num

number = 4
print(f"The square of {number} is {square(number)}.")
```
**Output:**  
```
The square of 4 is 16.
```

---

### **Multiline f-strings**  
f-strings can also be used with triple quotes for multiline output.  
```python
name = "Liam"
city = "London"

message = f"""
Hello {name},
Welcome to {city}!
Enjoy your stay.
"""
print(message)
```
**Output:**  
```
Hello Liam,
Welcome to London!
Enjoy your stay.
```

---

### **Exercises**  
#### **Exercise 1:** Basic f-string Formatting  
Write a program that takes two inputs: a name and an age. Then, display the message:  
```
Hello [name], you are [age] years old!
```

#### **Exercise 2:** Simple Math with f-strings  
Ask the user to input two numbers and display the result of their multiplication using f-strings.

#### **Exercise 3:** Temperature Conversion  
Write a program that asks for a temperature in Celsius and converts it to Fahrenheit using the formula:  
```
F = (C × 9/5) + 32
```
Use f-strings to display the result in a user-friendly way.

---


## Extra 03 Continued  


## Exercise 1: Receive the input of a multiplication of two numbers, check if its result higher than 100, then display if it is or not.  


## Exercise 2: Receive the input of three numbers and calculate their average.  


## Exercise 3: Receive 2 numbers, divide the first by the second one, then find the Remainder of the Division.  


## Exercise 4: Receive an number input for days, then convert it to hours, minutes and seconds.  


## Exercise 5: Receive inputs from the user asking for: name and middle name. Then print the first name, second name and full name sepparately.  


## Exercise 6: Find the Largest Number of two inputted numbers: Ask the user to input two numbers and print the largest one. If they are equal, display a message saying they are the same.  
  
