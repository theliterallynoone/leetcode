# COUNT VOWELS
# solution-
```
s=str(input("enter a string: "))
v= "AEIOUaeiou"
c=0
for i in s:
	if i in v:
		c+=1
print(c)
```
output-
```
enter a string: the quick brown fox jumps over the lazy little dog
13
```
