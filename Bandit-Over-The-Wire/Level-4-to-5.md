# Bandit Level 4 > 5

## Description:
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Tips to help to solve this Level:
ls, cd, cat, file, du, find

## Solution:
Here we have 1 directory /inhere with 10 files starting with -file going from 00 to 09. This is a 2 fold exercise, first you need to know how to open the contents of each file and 2nd which file has the password that is readable.

Steps:
1. Check Directory Contents
```bash
cd inhere
ls -al
```
2. This brings up the 10 files the directory has i.e. ```-file00``` to ```-file09```. Now the tricky part here is you can't directly open files beginning with `-`. So the step here was to check the data type of each file rather than going through each one.

```bash
file ./*
```

3. This displays the types and pinpoints the file that has a different type to all other files. 

```bash
./-file07: ASCII text
```

4. Last step was to simply read the contents of this file.
```bash
cat ./-file07
```

![](images/bandit4to5.png)
