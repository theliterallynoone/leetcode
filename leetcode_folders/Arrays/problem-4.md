# Problem- “Kids With the Greatest Number of Candies” (LeetCode #1431)

You’re given a list candies where candies[i] is how many candies kid i has.
You also get an integer extraCandies.

You must return a list of True/False, where True means:

“If that kid got the extra candies, they'd have the greatest number of candies among all kids.”

Example:
```
candies = [2, 3, 5, 1, 3]
extraCandies = 3
```

Max already is 5.

Check each kid:

Kid 0: 2 + 3 = 5 → True

Kid 1: 3 + 3 = 6 → True

Kid 2: 5 + 3 = 8 → True

Kid 3: 1 + 3 = 4 → False

Kid 4: 3 + 3 = 6 → True

So answer =
```
[True, True, True, False, True]
```

# Solution-

```
candies = list(map(int, input("Enter candies: ").split()))
extracandies = int(input("Enter extra candies: "))
max_c= max(candies)
result = []
for c in candies:
	if c+extracandies >= max_c:
		result.append(True)
	else:
		result.append(False)
print(result)
```

so then-

```
Enter candies: 9 8 7 6 5 4
Enter extra candies: 5
[True, True, True, True, True, True]
```


## Yay
