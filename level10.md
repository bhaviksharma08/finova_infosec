# Bandit 9 -> 10

## Challenge: Finding password in a file (data.txt) in one of the few human-readable strings, preceded by several ‘=’ characters.

### Command:
```bash
strings data.txt | grep "=="
```

### Explanation:
**```strings``` command:** Returns printable (human-readable) strings from a set of binary strings or a non-readable file
- The final command passes (pipes) human-readable strings to ```grep``` command, which then searches for strings which have more than one '=' in them.

### Output:
========== the
========== password
f\Z'========== is
========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

### Password:
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
