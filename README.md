
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
**Print-Working-Directory** `pwd` commands explore the filesytem.

### Tasks 5

Create a **Copy** `cp` of *science.txt* and call it *science.bak*. Recall the
`cp` command works as follows:

        cp /path/to/src /path/to/destination

Then **Move** `mv` the copy to the archive directory. The `mv` command works
much like the `cp` command where you will define a *target* file and a
*destination* like so,

        mv science.bak /path/to/archive-folder

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

1. Using pipes, display all lines of *list2*.

This can be done in several ways, these are some of them:

        cat -n list1 | grep -i "p"

OR in one command...

        grep -ni "p" list1

This can be taken further by using `sort` command.

        grep -ni "p" list1 | sort -t ':' -k2

The output of the `grep` command is sent into the `sort` program with the
options to consider `:` as a deliminter and to sort on the second field (`-k2`).
To send the output of the command above to a seperate file we can use `>` for
re-direction.


```less
cat -n list1

     1	orange,
     2	plum,
     3	mango,
     4	grapefruit

grep -ni "p" list1

    2:plum,
    4:grapefruit

grep -ni "p" list1 | sort -t ':' -k2

     4:grapefruit
     2:plum,

grep -i "p" list1 | sort -t ':' -k2

    grapefruit
    plum,
```

ii) Search the file *science.txt* for the word 'science', sort the output and
store it in a file.

        grep -i "science" science.txt | sort > task8-sorted-science.txt

### Tasks 9

A new (empty) file can be created using the `touch` command, like so;

`touch mynewfile.txt`

Then inspect the permissions of the file using:
`ls -la`

```less
-rw-r--r--  1 tarek_allam staff    0 Oct 12 22:52 mynewfile.txt
```

This can be changed using the **Change-Mode** `chmod` command:

`chmod u-r mynewfile.txt`

`ls -la`
```less
--w-r--r--  1 tarek_allam staff    0 Oct 12 22:52 mynewfile.txt
```

Notice this has rendered the file un-readable to the user. We can change this
back with:

`chmod u+r mynewfile.txt`

```less
-rw-r--r--  1 tarek_allam staff    0 Oct 12 22:52 mynewfile.txt
```

### Tasks 10
### Tasks 11
