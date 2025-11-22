# checking palindromes

# solution
```
l1= list(map(str, input("Enter list(separated by ',' please): ").split(",")))
pl1= l1[::-1]
if l1==pl1:
	print("yes")
else:
	print("no")
```
