# Bandit 6 -> 7

### Challenge: Finding a file with given conditions (size = 33 bytes, owned by user bandit7 and group bandit6)

**Command 1:**
```bash
find / -type f -user "bandit7" -group "bandit6" -size 33c 2>/dev/null
```

**Explanation:**
- The challenge says that the file is stored 'somewhere on the server' and not 'somewhere on the home directory' so we have to search the whole
root directory (/) on the server and not just the current directory (/home/bandit6)
- We want to remove the access permission denied errors from the output log, so redirecting output to /dev/null using '>' operator with the prefix of
2 (denoting stderr)

**Output:**
/var/lib/dpkg/info/bandit7.password

**Command 2:**
```bash
cat /var/lib/dpkg/info/bandit7.password
```

**Output:**
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

**Password:**
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
