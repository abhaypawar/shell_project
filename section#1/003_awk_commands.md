### awk

```sh
$ awk /manager018x/‘{print}’ raw_file.txt
#Prints anything that contains word manager018x anywhere in the given file.

$ awk '/error/' raw_file.txt
# Prints lines wherever contains error word in the given file.

$ awk -F ',' '{print $2}' users.csv
# Prints specific column 2 of each entry from file users.csv 

$ awk '/error/ {sub("error", "warning")} 1' errors.log
# Replaces error with warning. The 1 at the end is an empty action that ensures all lines are processed (since the search pattern might not match all lines).

$ awk '{print toupper($1)}' names.txt
# This command iterates through "names.txt" and applies the toupper function to the first field ($1) of each line. It prints the resulting uppercase version.
```

Try yourself -
```sh
$ hello=devops=sre
$ echo $hello | sed ‘s/=/ /g’ | awk ‘{print $2}’
```
