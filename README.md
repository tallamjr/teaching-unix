
# Notes

## Introduction to UNIX

### UNIX

Written with the `C` language.


## Tasks

### Tasks 1

What does this tell you about the way the shell works?

    This shows that each shell has it's own set of variables and can work
    independently from the other shells.

### Tasks 2

**Print-Working-Directory**

`$ pwd`

**Make-Directory** called *unixstuff*

`$ mkdir unixstuff`

### Tasks 3

Go into that directory and create another directory called *archive*, so,
**Change-Directory** to the recently create directory called *unixstuff*

`$ cd unixstuff`

and **Make-Directory** called *archive*

`$ mkdir archive`

### Tasks 4

Using the **Change-Directory** `cd`, **List** `ls` and
**Print-Working-Directory** commands explore the filesytem.

### Tasks 5

Create a **Copy** `cp` of *science.txt* and call it *science.bak*. Recall the
`cp` command works as follows:

        `cp /path/to/src /path/to/destination`

Then **Move** `mv` the copy to the archive directory. The `mv` command works
much like the `cp` command where you will define a *target* file and a
*destination* like so,

        `mv science.bak /path/to/archive-folder`

### Tasks 6

**Make-Directory** called *tempstuff* using `mkdir`. **Copy** *science.txt* to
*tempstuff* using `cp`. Then **Remove-Directory** using `rmdir`. If the folder
is not empty, then `rm -r` is required. The `-r` flag refers to remove files
recursively

### Tasks 7

```bash
echo "orange, plum, mango, grapefruit." > list2
```

OR

```bash
vim list2
```
Using the `vim` terminal editor, type the following inside:

`orange, plum, mango, grapefruit.`

and then save with `<Shift>ZZ`

### Tasks 8

### Tasks 9
### Tasks 10
### Tasks 11
