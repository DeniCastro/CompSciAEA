## What are Logic Gates?


Logic gates are small electronic components that take binary inputs (0 or 1) and produce a binary output. They are used in all modern digital systems.

---

## What are Binary Inputs and Outputs?

- **Binary Input**: A signal that can only be 0 (off) or 1 (on)
- **Binary Output**: The result from the logic gate, also 0 or 1

---

## How Do Logic Gates Work?

Each gate follows a specific rule. For example:

- **NOT gate**: Inverts the input  
  - Input: 1 → Output: 0  
  - Input: 0 → Output: 1

- **AND gate**: Output is 1 only if both inputs are 1  
- **OR gate**: Output is 1 if at least one input is 1

---

## Example: AND Gate Truth Table

| A | B | Output |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   0    |
| 1 | 0 |   0    |
| 1 | 1 |   1    |

---

## How to Understand Them

- Use **truth tables** to see input/output patterns
- Practice building **logic circuits**
- Learn the meanings of each gate (AND, OR, NOT, etc.)
  
# Introduction to Logic Gates and Logic Circuits

Electronic circuits found in computers, solid-state drives, and control devices are made up of thousands of logic gates. 

Logic gates work with **binary inputs** (0s and 1s) and produce a **binary output**. When several logic gates are connected together, they form a **logic circuit**, which is designed to carry out a specific task or function.

To check how a logic gate or logic circuit behaves, we use a **truth table**. A truth table lists all possible input combinations and shows the corresponding output.

This chapter will cover:
- The function and role of logic gates
- How logic circuits work
- How to use truth tables
- Examples of real-world application circuits

You will also see references to **Boolean algebra**. While this topic is more advanced and goes beyond the scope of this textbook, it is included for completeness. Boolean algebra appears frequently on websites and resources about logic gates, and some students may prefer its notation instead of standard logic statements.  



## 1. Standard Logic Gates

### NOT Gate
- **Definition**: The NOT gate (also called an inverter) outputs the opposite (inverse) of the input.
- **Symbol**: `¬` or `!`
- **Logic Symbol**:


  - **Function**: If input A is 1, output is 0; if input A is 0, output is 1.

| A | Q (¬A) |
|---|--------|
| 0 |   1    |
| 1 |   0    |

---

### AND Gate
- **Definition**: The AND gate outputs 1 only if all inputs are 1.
- **Symbol**: `∧` or `·`
- **Logic Symbol**:


- **Function**: Output is 1 when A or B or both are 1.

| A | B | Q (A ∨ B) |
|---|---|-----------|
| 0 | 0 |     0     |
| 0 | 1 |     1     |
| 1 | 0 |     1     |
| 1 | 1 |     1     |

---

### NAND Gate
- **Definition**: NAND is the opposite of AND. It outputs 0 only when all inputs are 1.
- **Symbol**: `¬(A ∧ B)`
- **Logic Symbol**:

- **Function**: Inverse of the AND gate.

| A | B | Q (¬(A ∧ B)) |
|---|---|--------------|
| 0 | 0 |      1       |
| 0 | 1 |      1       |
| 1 | 0 |      1       |
| 1 | 1 |      0       |

---

### NOR Gate
- **Definition**: NOR is the opposite of OR. It outputs 1 only when all inputs are 0.
- **Symbol**: `¬(A ∨ B)`
- **Logic Symbol**:  


 - **Function**: Inverse of the OR gate.

| A | B | Q (¬(A ∨ B)) |
|---|---|--------------|
| 0 | 0 |      1       |
| 0 | 1 |      0       |
| 1 | 0 |      0       |
| 1 | 1 |      0       |

---

### XOR Gate (Exclusive OR)
- **Definition**: Outputs 1 if the inputs are different.
- **Symbol**: `A ⊕ B`
- **Logic Symbol**:



  - **Function**: Output is 1 when A and B are different.

| A | B | Q (A ⊕ B) |
|---|---|-----------|
| 0 | 0 |     0     |
| 0 | 1 |     1     |
| 1 | 0 |     1     |
| 1 | 1 |     0     |

---

## 2. Creating Logic Circuits

### a) From a Given Problem
**Problem**: A light should turn on only when both switches A and B are on.

**Solution**: Use an AND gate.  
**Expression**: `A ∧ B`

---

### b) From a Logic Expression
**Expression**: `(A ∨ B) ∧ ¬C`

**Circuit**:
- Use an OR gate for A and B.
- Use a NOT gate for C.
- Use an AND gate to combine the OR and NOT outputs.

---

### c) From a Truth Table

| A | B | Q |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

This is the truth table of an XOR gate.  
**Expression**: `A ⊕ B`  
**Circuit**: Use a single XOR gate.

---

## 3. 10.1 Standard Logic Gate Symbols

| Gate | Symbol | Description |
|------|--------|-------------|
| NOT  | ¬A or !A | Inverts the input |
| AND  | A ∧ B or A · B | Output is 1 only when both inputs are 1 |
| OR   | A ∨ B or A + B | Output is 1 when at least one input is 1 |
| NAND | ¬(A ∧ B) | Output is 0 only when both inputs are 1 |
| NOR  | ¬(A ∨ B) | Output is 1 only when both inputs are 0 |
| XOR  | A ⊕ B | Output is 1 when inputs are different |

---
[Learn more about boolean logic and boolean algebra here (Crash Course YouTube)](https://www.youtube.com/watch?v=gI-qXk7XojA&ab_channel=CrashCourse)


   
