<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/7.9%20Writing%20and%20amending%20algorithms.jpg" alt="7.19" width="800"> 
</div>       
  
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Figure%207.18.jpg" alt="Figure 7.18" width="800"> 
</div>       
  
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Figure%207.19.jpg" alt="FIgure 7.19" width="800"> 
</div>     

# Writing algorithms in pseudocode    
### Video: [7.9 Amending Algorithms](https://www.youtube.com/watch?v=-s6xP2gYvxc)




Tickets are sold for a concert at 20$ each. If 10 tickets are bought then the discount is 10%, if 20 tickets are bought the discount is 20%. No more than 25 tickets can be bought in a single transaction.

A. Use a pseudocode to write the algorithm to calculate the cost of buying a given number of tickets.  

### Problem Statement

Tickets are sold for a concert at $20 each. The following discount rules apply:

- If **10 tickets** are bought, there is a **10%** discount.
- If **20 tickets** are bought, there is a **20%** discount.
- No more than **25 tickets** can be bought in a single transaction.

The goal is to create an algorithm in pseudocode to calculate the total cost of purchasing a given number of tickets.

---


 
## Step-by-Step Breakdown

### 1. Input the Number of Tickets
Prompt the user to enter how many tickets they want to buy.

```
OUTPUT "Enter the number of tickets:"
INPUT tickets
```

### 2. Validate the Input
Ensure the number of tickets is within the allowed range (1 to 25).

```
IF tickets < 1 OR tickets > 25 THEN
    OUTPUT "Invalid number of tickets. Must be between 1 and 25."
    END
```

### 3. Set the Ticket Price
Define the cost of a single ticket as $20.

```
SET price_per_ticket = 20
```

### 4. Apply the Discount
Check how many tickets were purchased and apply the corresponding discount.

```
IF tickets >= 20 THEN
    SET discount = 0.20
ELSE IF tickets >= 10 THEN
    SET discount = 0.10
ELSE
    SET discount = 0
```

### 5. Calculate the Total Cost
Compute the total cost by multiplying the number of tickets by the price per ticket, then applying the discount.

```
SET total_cost = tickets * price_per_ticket
SET total_cost = total_cost - (total_cost * discount)
```

### 6. Display the Final Cost
Output the final price after any applicable discounts.

```
OUTPUT "Total cost: $", total_cost
```

---

## Complete Pseudocode

```
OUTPUT "Enter the number of tickets:"
INPUT tickets

IF tickets < 1 OR tickets > 25 THEN
    OUTPUT "Invalid number of tickets. Must be between 1 and 25."
    END

SET price_per_ticket = 20

IF tickets >= 20 THEN
    SET discount = 0.20
ELSE IF tickets >= 10 THEN
    SET discount = 0.10
ELSE
    SET discount = 0

SET total_cost = tickets * price_per_ticket
SET total_cost = total_cost - (total_cost * discount)

OUTPUT "Total cost: $", total_cost
```

---

## Example Outputs

### Example 1: Valid Input (15 Tickets)
```
Enter the number of tickets: 15  
If the tickets are 20$ and 15 * 20 = 300
300 is multiplied by the discount (300 * 0,10), which totalizes 30
Then you subtract 300 (initially the full price) by the discount (30)
Total cost: $270.0
```

### Example 2: Valid Input (25 Tickets)
```
Enter the number of tickets: 25
Total cost: $400.0
```

### Example 3: Invalid Input (30 Tickets)
```
Enter the number of tickets: 30
Invalid number of tickets. Must be between 1 and 25.
```

# Shopping Discount Calculation Algorithm

Customers shopping at a store receive discounts based on their total purchase amount. The store applies the following discount rules:

- **No discount** if the total amount is less than $50.
- **5% discount** if the total amount is between $50 and $99.
- **10% discount** if the total amount is between $100 and $199.
- **15% discount** if the total amount is $200 or more.

## **Step-by-Step Explanation**

1. **Prompt the user for the total purchase amount.**
2. **Check the amount against the discount rules.**
3. **Apply the corresponding discount based on the amount.**
4. **Calculate the final cost after the discount.**
5. **Display the discounted amount and final price.**

## **Pseudocode**

```
BEGIN
    PROMPT "Enter total purchase amount: "
    INPUT totalAmount

    IF totalAmount >= 200 THEN
        discountRate ← 15
    ELSE IF totalAmount >= 100 THEN
        discountRate ← 10
    ELSE IF totalAmount >= 50 THEN
        discountRate ← 5
    ELSE
        discountRate ← 0
    ENDIF

    discount ← (totalAmount * discountRate) / 100
    finalCost ← totalAmount - discount

    OUTPUT "Total Amount: $" totalAmount
    OUTPUT "Discount Applied: " discountRate "%"
    OUTPUT "Final Cost: $" finalCost
END
```

## **Example Output**

```
Enter total purchase amount: 120
Total Amount: $120
Discount Applied: 10%
Final Cost: $108
```

[Use this pseudocode compiler online.](https://pseudocode.deepjain.com/)

## **Practice Task**

1. Modify the algorithm to apply a **25% discount** if the amount exceeds **$500**.
2. Add a condition to **prevent negative inputs** and display an error message if the input is invalid.
3. Enhance the output to show both the **discount amount** and the **final price** clearly.
