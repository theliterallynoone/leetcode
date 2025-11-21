# Problem #5- Concatenation of Array

You're given an array ```nums```.
Return an array ```ans``` such that:

```
ans = nums + nums
```

Example:
```
[1,2,1] → [1,2,1,1,2,1]
```

# Solution-
```
nums= list(map(int, input("Enter list(separated by ',' please): ").split(",")))
ans= nums+nums
print(ans)
```
So the output becomes-
```
Enter list(separated by ',' please): 4,5,6,2 
[4, 5, 6, 2, 4, 5, 6, 2]
```
