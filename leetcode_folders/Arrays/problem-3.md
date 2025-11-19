# Problem #3 — Richest Customer Wealth

Difficulty: Easy
Category: Arrays / 2D Arrays

# 📌 Problem

You’re given a 2D list accounts, where each row is a customer and each value is money in a bank.
Find which customer has the maximum total money.

Example:
Input-
[[1,5],[7,3],[3,5]] 
→ sums = [6, 10, 8]
→ answer = 10 (output)

# Solution-

```
def maximumwealth(acc):
    max_wealth = 0

    for customer in acc:
        w = sum(customer)
        if w > max_wealth:
            max_wealth = w
    return max_wealth
        
#to test this-
acc = ([8,9],[5,4,8],[7,2,3])
print(maximumwealth(acc))
```

which gives the output as- 
# 17
