# Filtering and finding files based on a given set of conditions
### 'find' command: Searches the given directory and all the sub-directories for files satisfying the given conditions.  Syntax: find <directory_name> \<parameter> <argument_value>
### Arguments used:
- **-size**: This argument takes a value or a range of values of the file size
- **-type**: Takes file type as parameter
- **-executable**: Specifies that the file is executable. Applying a '!' operator before this argument reverses the condition, stating that the file should be non-executable.
# Linux command:
```find . -type f -readable -size 1033c ! -executable```
