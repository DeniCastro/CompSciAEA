# **Validation and Verification in Python**  

When we enter data into a computer system, we must ensure that it is **reasonable** and **accurate**. There are two ways to check this:  

1️⃣ **Validation** – Checking if the data is reasonable before accepting it.  
2️⃣ **Verification** – Ensuring data is not changed while being entered.  

---

## **1. Validation**  
Validation is when the computer automatically checks whether the input **makes sense**. If the data is incorrect, the system should display an error message and ask the user to re-enter the data.

There are different **types of validation checks**:

- ✅ **Range Check** – Ensures a value is within a certain range (e.g., a student's mark is between 0 and 100).  
- ✅ **Length Check** – Ensures the number of characters is correct (e.g., a phone number must have 10 digits).  
- ✅ **Type Check** – Ensures the input is the correct data type (e.g., a mark must be a number, not text).  
- ✅ **Presence Check** – Ensures that the user enters some data (e.g., a name cannot be left blank).  
- ✅ **Format Check** – Ensures data follows a specific pattern (e.g., an email must have **@** and **.com**).  

---

### **Range Check Example**  
The following **pseudocode** checks if a student's mark is between **0 and 100**:

```plaintext
OUTPUT "Please enter the student's mark"
REPEAT
    INPUT StudentMark
    IF StudentMark < 0 OR StudentMark > 100 THEN
        OUTPUT "The student's mark should be between 0 and 100. Please re-enter."
    ENDIF
UNTIL StudentMark >= 0 AND StudentMark <= 100
