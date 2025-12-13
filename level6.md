# Filtering and finding files based on a given set of conditions
### 'find' command: Searches the given directory and all the sub-directories for files satisfying the given conditions.  Syntax: find <directory_name> \<parameter> <argument_value>
### Arguments used:
- **-size**: This argument takes a value or a range of values of the file size
- **-type**: Takes file type as parameter
- **-executable**: Specifies that the file should be executable. Applying a '!' operator before this argument reverses the condition, stating that the file should be non-executable.
- **-readable**: Specifies that the file should be readable.
# Linux command:
```find . -type f -readable -size 1033c ! -executable```

- "-type f": Implies that this is a file, not a directory or a symbolic link
- 1033c: Size is 1033 bytes (c indicates bytes, k indicates kilobytes)
