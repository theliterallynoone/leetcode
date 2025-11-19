# Arrays
problem 1:

# ⭐ **Problem #1 - Running Sum of 1D Array**

Difficulty: *Easy*

Category: **Arrays**

### 📌 Problem

Given an array `nums`, return an array where each element is the **running sum** so far.

Example:

```
Input:  [1, 2, 3, 4]
Output: [1, 3, 6, 10]
```

Another:

```
Input:  [1, 1, 1, 1, 1]
Output: [1, 2, 3, 4, 5]
```

---

# solution 
```
def runningSum(nums):
    result = []
    current_sum = 0

    for x in nums:
        current_sum = current_sum + x
        result.append(current_sum)

    return result
    
print(runningSum([7,8,9,10]))
```

so the output we get becomes-
# [7, 15, 24, 34]
