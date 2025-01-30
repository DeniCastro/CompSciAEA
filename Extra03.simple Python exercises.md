# 📝 Basic Python Exercises for Beginners

## 1️⃣ Understanding Even and Odd Numbers
Before checking if a number is odd or even, remember:
- A number is **even** if it is divisible by 2 (i.e., `number % 2 == 0`).  
- A number is **odd** if it is **not** divisible by 2 (i.e., `number % 2 != 0`).  

### 🛠 **Exercise:**
Write a Python program that asks the user for a number and prints whether it is odd or even.

```python
# Get user input
number = int(input("Enter a number: "))

# Check if the number is even or odd
if number % 2 == 0:
    print("The number is even.")
else:
    print("The number is odd.")
```

---

## 2️⃣ Prime or Composite Numbers
A **prime number** is a number greater than 1 that has only two factors: **1 and itself**.  
A **composite number** has more than two factors.  

To check if a number is prime:
1. Divide it by numbers from `2` to `number - 1`.
2. If it is divisible by any of them, it is **not** prime.

### 🛠 **Exercise:**
Write a Python program that takes an integer input and determines if it is prime or composite.

```python
# Get user input
num = int(input("Enter a number: "))

# Check if the number is prime
if num > 1:
    for i in range(2, num):
        if num % i == 0:
            print("The number is composite.")
            break
    else:
        print("The number is prime.")
else:
    print("The number is neither prime nor composite.")
```

---

## 3️⃣ Simple Calculator
Before creating a calculator, understand that:
- We use operators: `+`, `-`, `*`, `/` for basic arithmetic.
- We need user input for numbers and the operation type.

### 🛠 **Exercise:**
Write a Python program that asks the user to input two numbers and an operator (`+`, `-`, `*`, or `/`). Then, perform the calculation and display the result.

```python
# Get user input
num1 = float(input("Enter first number: "))
operator = input("Enter an operator (+, -, *, /): ")
num2 = float(input("Enter second number: "))

# Perform calculation
if operator == '+':
    print("Result:", num1 + num2)
elif operator == '-':
    print("Result:", num1 - num2)
elif operator == '*':
    print("Result:", num1 * num2)
elif operator == '/':
    if num2 != 0:
        print("Result:", num1 / num2)
    else:
        print("Error: Division by zero is not allowed.")
else:
    print("Error: Invalid operator.")
```

---

## 4️⃣ Finding the Largest Number
To compare numbers, we use the **`max()` function** or conditional statements.

### 🛠 **Exercise:**
Write a Python program that takes three numbers from the user and prints the largest one.

```python
# Get user input
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
num3 = float(input("Enter third number: "))

# Find the largest number
largest = max(num1, num2, num3)
print("The largest number is:", largest)
```

---

## 5️⃣ FizzBuzz Challenge
**FizzBuzz** is a common coding test question:
- If a number is divisible by `3`, print `"Fizz"`.
- If a number is divisible by `5`, print `"Buzz"`.
- If a number is divisible by **both** `3` and `5`, print `"FizzBuzz"`.
- Otherwise, print the number itself.

### 🛠 **Exercise:**
Write a Python program that asks the user for a number and applies the **FizzBuzz** rules.

```python
# Get user input
num = int(input("Enter a number: "))

# Apply FizzBuzz rules
if num % 3 == 0 and num % 5 == 0:
    print("FizzBuzz")
elif num % 3 == 0:
    print("Fizz")
elif num % 5 == 0:
    print("Buzz")
else:
    print(num)
