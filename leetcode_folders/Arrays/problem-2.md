# Problem #2 — Find Pivot Index

Difficulty: Easy
Category: Arrays / Prefix Sums

# 📌 Problem

Given an array nums, return the pivot index.

The pivot index is the spot where:

sum of all numbers to the left = sum of all numbers to the right

Example:

Input:  [1, 7, 3, 6, 5, 6]
Output: 3 [indexing]   (because left sum = 1+7+3= 11, right sum = 5+6= 11)


If no pivot exists → return -1.

# SOLUTION

```
def pivotindex(num):
		total = sum(num)
		l_s=0
		
		for i in range(len(num)):
				r_s = total - l_s - num[i]
				if l_s == r_s:
                    return i #pivot found
				l_s += num[i] #updated left sum
				
		return -1
		
#and now, to test this monsieur
print(pivotindex([8,9,5,1,2,5,5,5,5,5]))
```

so the output we get becomes-
# -1

or if we try a different print statement, maybe one with another 5- 
```
print(pivotindex([8,9,5,1,2,5,5,5,5,5,5]))
```
the output becomes-
# 5
