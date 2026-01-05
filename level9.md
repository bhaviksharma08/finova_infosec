# Bandit 8 -> 9

## Challenge: Searching for a substring within a file that occurs only once

## Command:
```bash
sort data.txt | uniq -u
```

## Explanation:
### ```sort``` command:
- Sorts lines of text in the given file based on given parameters. By default, sorts lines alphabetically (lexicographically).
- This also means that duplicate lines will be arranged next to each other.
- This works well with ```uniq``` command which returns 'consecutively recurring lines'
- ```-u``` parameter with ```uniq``` command specifies to print only those that are unique (occur only once and do not repeat consec)

**Output (Password):**
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
