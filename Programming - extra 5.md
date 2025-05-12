# Arrays in Python

In Python, arrays can be implemented in multiple ways. The most common are:

- Using **lists**, which are built-in and dynamic.
- Using the **array module**, which is more efficient for numeric values of the same type.

---

## 1. Using Lists (Built-in Arrays)

Python lists are flexible and can hold any data type.

### Example: Creating and accessing a list

```python
# Creating a list
fruits = ["apple", "banana", "cherry"]

# Accessing elements
print(fruits[0])  # Output: apple

# Modifying elements
fruits[1] = "blueberry"

# Adding elements
fruits.append("date")

# Removing elements
fruits.remove("cherry")

# Looping through a list
for fruit in fruits:
    print(fruit)
```
## 2. Using the array Module
The array module is better when working with large numeric datasets.

```python
import array

# array(typecode, initializer)
a = array.array('i', [1, 2, 3, 4])
```
  
### Example using the ARRAY module:
```python  
import array

# Create an integer array
numbers = array.array('i', [10, 20, 30])

# Append an item
numbers.append(40)

# Access and modify
print(numbers[2])  # Output: 30
numbers[1] = 25

# Iterate
for num in numbers:
    print(num)
```
