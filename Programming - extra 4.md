# Understanding Functions in Python

## Introduction to Functions

### What is a Function?
A function is a reusable block of code that performs a specific task. Functions help break a program into smaller parts, making it easier to understand, debug, and maintain.

### Why Use Functions?
- **Reusability:** Write the code once and use it multiple times.
- **Readability:** Makes programs easier to read and understand.
- **Organization:** Helps structure programs into logical sections.
- **Efficiency:** Reduces repetition and avoids errors.

---

## Basics of Functions

### Defining and Calling Functions
To create a function in Python, we use the `def` keyword.

```python
# Defining a function
def greet():
    print("Hello, welcome to Python programming!")

# Calling the function
greet()
```

### Function with Parameters
Functions can accept inputs (parameters) to perform specific tasks.

```python
# Function with a parameter
def greet(name):
    print(f"Hello, {name}! Welcome to Python programming.")

# Calling the function with an argument
greet("Alice")
```

### Function with Multiple Parameters

```python
def add_numbers(a, b):
    result = a + b
    print(f"The sum of {a} and {b} is {result}")

add_numbers(5, 3)
```

### Return Statement
A function can return a value instead of printing it.

```python
def multiply(a, b):
    return a * b

result = multiply(4, 5)
print("The product is", result)
```

---

## Advanced Function Concepts

### Default Parameter Values

```python
def greet(name="Student"):
    print(f"Hello, {name}!")

greet()  # Uses the default value
greet("Bob")  # Overrides the default value
```

### Keyword Arguments

```python
def introduce(name, age):
    print(f"My name is {name} and I am {age} years old.")

introduce(age=25, name="Alice")  # Order doesn't matter
```

### Functions with Lists

```python
def find_max(numbers):
    return max(numbers)

values = [10, 20, 5, 40, 25]
print("The maximum value is", find_max(values))
```

### Functions Calling Other Functions

```python
def square(num):
    return num * num

def cube(num):
    return num * square(num)

print("The cube of 3 is", cube(3))
```

---

## Recursion and Lambda Functions

### Recursive Functions
A recursive function is a function that calls itself to solve a smaller version of a problem.

```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

print("Factorial of 5 is", factorial(5))
```

### Lambda Functions
A lambda function is a short function that has no name.

```python
# Regular function
def square(x):
    return x * x

# Lambda function
y = lambda x: x * x

print("Square of 5 is", y(5))
```

---

## Exercises
### **Basic Exercises**
1. Write a function that prints "Good morning!".
2. Create a function that takes a number and returns its square.
3. Write a function that takes two numbers and returns their difference.

### **Intermediate Exercises**
4. Write a function that takes a list of numbers and returns the largest one.
5. Create a function that checks if a number is even or odd.

### **Advanced Exercises**
6. Write a recursive function to calculate the sum of the first `n` natural numbers.
7. Implement a function that takes a string and returns it in reverse order using recursion.

---

# Advanced Function Parameters and Return Types

## Positional vs. Keyword Arguments
# Positional arguments must be given in order.  


```python  
def greet(name, message):
    print(f"{message}, {name}!")

greet("Alice", "Hello")  # Correct
#greet("Hello", "Alice")  # Incorrect order!

## Default Parameters
# If a parameter is not given, the default value is used.
def greet(name, message="Hi"):
    print(f"{message}, {name}!")

greet("Bob")  # Uses default message "Hi"
greet("Bob", "Good morning")  # Custom message

## Returning Multiple Values
def divide_numbers(a, b):
    quotient = a // b
    remainder = a % b
    return quotient, remainder  # Returns a tuple

q, r = divide_numbers(10, 3)
print(f"Quotient: {q}, Remainder: {r}")

```


# Higher-Order Functions and Lambda Expressions

```python  
## Functions as Arguments
def apply_operation(x, y, operation):
    return operation(x, y)

def add(a, b):
    return a + b

def multiply(a, b):
    return a * b

print(apply_operation(3, 4, add))  # Passes 'add' function
print(apply_operation(3, 4, multiply))  # Passes 'multiply' function
``` 

## Lambda Functions (anonymous functions)  

``` square = lambda x: x * x
print(square(5))  # Output: 25

```  


## Using map(), filter(), reduce()  

```python 
from functools import reduce
numbers = [1, 2, 3, 4, 5]

doubled = list(map(lambda x: x * 2, numbers))  # Applies function to all items
print(doubled)

even_numbers = list(filter(lambda x: x % 2 == 0, numbers))  # Keeps only even numbers
print(even_numbers)

sum_total = reduce(lambda x, y: x + y, numbers)  # Reduces list to single value
print(sum_total)
``` 


# Recursion and Function Scope  

## Recursion: A function that calls itself    

```python 
def factorial(n):
    if n == 1:
        return 1  # Base case
    return n * factorial(n - 1)  # Recursive case

print(factorial(5))  # 5! = 5*4*3*2*1 = 120

## Local vs. Global Variables
global_var = "I'm global"

def example():
    local_var = "I'm local"
    print(global_var)  # Accessible
    print(local_var)  # Accessible

example()
#print(local_var)  # ERROR: Not accessible outside function
``` 


## Nested Functions & Closures

```python 

def outer_function():
    message = "Hello"
    def inner_function():
        print(message)  # Inner function can access 'message'
    return inner_function

my_func = outer_function()
my_func()  # Prints "Hello"
``` 


