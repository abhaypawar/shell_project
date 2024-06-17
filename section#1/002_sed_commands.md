### Stream Editor
In vim commands we go inside the file and then edit the part, but here in sed commands we can edit without going inside the file. That means better Automation!

```sh
$sed -n ‘1-3’ p raw_file.txt
#Prints first three lines from raw_file.txt

$sed ‘s/warnings/errors/g’ abhay_files.txt
#Substitutes globally warnings -> with errors in given file. If g not given, just the first value will be substituted.
```
