# Algorithms


An **algorithm** is a step-by-step set of instructions to solve a problem. Think of it like a recipe: you follow the steps to make a dish, just like a computer follows an algorithm to solve a problem.

## Conditional Statements (IF-ELSE)
Conditional statements help computers make decisions.

### Example in Pseudocode:
```
OUTPUT "Enter your age:"
INPUT Age
IF Age >= 18 THEN
    OUTPUT "You are an adult."
ELSE
    OUTPUT "You are a minor."
ENDIF
```

### Example in Python:
```python
age = int(input("Enter your age: "))
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

## Finding Maximum, Minimum, and Average
### Purpose:
- **Maximum**: Finds the highest number.
- **Minimum**: Finds the lowest number.
- **Average**: Calculates the total and divides by the number of values.

### Example in Pseudocode:
```
Maximum ← Numbers[1]
Minimum ← Numbers[1]
Total ← 0
FOR Counter ← 1 TO Length
    IF Numbers[Counter] > Maximum THEN
        Maximum ← Numbers[Counter]
    ENDIF
    IF Numbers[Counter] < Minimum THEN
        Minimum ← Numbers[Counter]
    ENDIF
    Total ← Total + Numbers[Counter]
NEXT Counter
Average ← Total / Length
OUTPUT "Maximum:", Maximum
OUTPUT "Minimum:", Minimum
OUTPUT "Average:", Average
```

### Example in Python:
```python
numbers = [10, 25, 5, 40, 15]
maximum = numbers[0]
minimum = numbers[0]
total = 0

for num in numbers:
    if num > maximum:
        maximum = num
    if num < minimum:
        minimum = num
    total += num

average = total / len(numbers)
print("Maximum:", maximum)
print("Minimum:", minimum)
print("Average:", average)
```

## Linear Search
### Purpose:
A **linear search** is used to find a value in a list by checking each item one by one.

### Example in Pseudocode:
```
OUTPUT "Enter number to search for:"
INPUT SearchValue
Found ← False
Counter ← 1
REPEAT
    IF Numbers[Counter] = SearchValue THEN
        Found ← TRUE
    ELSE
        Counter ← Counter + 1
    ENDIF
UNTIL Found OR Counter > Length
IF Found THEN
    OUTPUT "Number found at position:", Counter
ELSE
    OUTPUT "Number not found."
ENDIF
```

### Example in Python:
```python
numbers = [3, 7, 12, 18, 25]
search_value = int(input("Enter number to search for: "))
found = False

for index in range(len(numbers)):
    if numbers[index] == search_value:
        found = True
        print("Number found at position:", index + 1)
        break

if not found:
    print("Number not found.")
```

## Bubble Sort
### Purpose:
Bubble Sort is a way to **arrange numbers in order** by comparing and swapping them if they are in the wrong order.

### Example in Pseudocode:
```
First ← 1
Last ← Length
REPEAT
    Swap ← False
    FOR Index ← First TO Last - 1
        IF Numbers[Index] > Numbers[Index + 1] THEN
            Temp ← Numbers[Index]
            Numbers[Index] ← Numbers[Index + 1]
            Numbers[Index + 1] ← Temp
            Swap ← TRUE
        ENDIF
    NEXT Index
    Last ← Last -1
UNTIL NOT Swap OR Last = 1
```

### Example in Python:
```python
numbers = [5, 3, 8, 1, 2]
n = len(numbers)

for i in range(n-1):
    swapped = False
    for j in range(n-1-i):
        if numbers[j] > numbers[j+1]:
            numbers[j], numbers[j+1] = numbers[j+1], numbers[j]
            swapped = True
    if not swapped:
        break

print("Sorted list:", numbers)
```

---

