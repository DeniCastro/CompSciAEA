# Basic Python Instructions

## 1. How to Add a Comment
Comments are lines that Python ignores. They are useful for explaining code.

```python
# This is a comment
# Comments start with a # symbol
```

## 1.2 Data types 
<div align="center">
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Picture2.jpg" alt="Data types" width="500"> 
</div>   


## 2. What is a Variable and Why It Needs a Name
A **variable** is a way to store data. It must have a **name** so we can use it later.

```python
name = "Alice"  # 'name' is the variable, "Alice" is its value
age = 25  # 'age' is the variable, 25 is its value
```

### Why does a variable need a name?
- So we can reference and modify it later.
- It helps make the code more readable.

## 3. How to Make an Input That Receives a Variable
We use the `input()` function to get user input.

```python
name = input("Enter your name: ")  # Stores the user's input in 'name'
print("Hello, " + name + "!")  # Prints a greeting
```

If we want a number as input, we convert it to an integer:

```python
age = int(input("Enter your age: "))  # Converts input to an integer
print("You are", age, "years old.")
```

## 4. Difference Between `if`, `elif`, and `else`
These are used for decision-making in Python.

```python
age = int(input("Enter your age: "))

if age < 18:  # 'if' checks the first condition
    print("You are a minor.")
elif age == 18:  # 'elif' (else if) checks another condition
    print("You just became an adult!")
else:  # 'else' runs if none of the above conditions are met
    print("You are an adult.")
```

### Note: Python does **not** use `endif` like some other languages.
Instead, it uses indentation to mark the end of an `if` block.

---

