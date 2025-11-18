# Arrays
problem 1:

# ⭐ **Warmup Problem: Running Sum of 1D Array**

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

# 🎯 Your Goal

1. Think about how you’d compute the running sum.
2. Then write the code in python.



# solution 

def runningSum(nums):
    result = []
    current_sum = 0

    for x in nums:
        current_sum = current_sum + x
        result.append(current_sum)

    return result
    
print(runningSum([1, 2, 3, 4]))


