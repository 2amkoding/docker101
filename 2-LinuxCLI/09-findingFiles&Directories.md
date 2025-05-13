```plaintext

find            : recursively list all files and directories
find -type d    : to list directories only
find -type f    : to list files only
find -name “f*” : to filter by name using a pattern

find -type f -iname "f*"
find -type f -name "*py"

## notes
 ls : by default !shows hidden files
 ls -a: includes hidden files+directories
 find : shows hidden files+directories

```