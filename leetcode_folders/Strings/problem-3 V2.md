## Frequency of each vowel (a little stats moment)
```
s = input("Enter a string: ").lower()
freq = {v:0 for v in "aeiou"}

for ch in s:
    if ch in freq:
        freq[ch] += 1

print(freq)
```

so the output becomes
```
Enter a string: the quick brown fox jumps over the lazy little dog
{'a': 1, 'e': 4, 'i': 2, 'o': 4, 'u': 2}
```
