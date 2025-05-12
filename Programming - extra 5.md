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
