# File Commands
Guide for commands when working with files and folders.

This is based on Ubuntu 22.04.

## Folders
Create a new folder

```bash
mkdir <folder>
```

Delete a folder

```bash
rmdir <folder>
```

Delete a folder and all its contents

```bash
rm -rf <folder>
```

## Files

Create a new file

```bash
touch <file>
```

Delete a file

```bash
rm <file>
```

Copy a file

```bash 
cp <file> <new-file>
```

Move a file (or rename it)

```bash
mv <file> <new-file>
```

## View File Contents

View the contents of a file

```bash
cat <file>
```

View the contents of a file with line numbers

```bash
cat -n <file>
```

View the contents of a file one page at a time

```bash
less <file>
```

Show the first X lines of a file

```bash
head -n <number-of-lines> <file>
```

Show the last X lines of a file

```bash
tail -n <number-of-lines> <file>
```

Show the end of a file as it is being updated

```bash
tail -f <file>
```

## Find Files

Find files in the current folder and subfolders

```bash
find . -name <file pattern>
```

Note: use -iname to ignore case

## Compare Files

Compare two files

```bash
diff <file1> <file2>
```

Use -i to ignore case, -w to ignore whitespace.

Use diff3 command to compare 3 files:
    
```bash
diff3 <file1> <file2> <file3>
```

To create a "patch file" with the differences between 2 files:
    
```bash
diff -u <file1> <file2> > <patch-file>
```

Use patch command to apply the patch file to the original file:
    
```bash
patch <file1> < <patch-file>
```

To patch a folder of files:
    
```bash
diff -Nur <original-folder> <new-folder> > <patch-file>
```

Use patch command to apply the patch file to the original folder:
    
```bash
patch -p1 < <patch-file>
```

## File Permissions

Change the permissions of a file or folder

```bash
chmod <permissions> <file>
```

Permissions is a 3 digit number, where each digit is a sum of the following values:

- 4 = read
- 2 = write
- 1 = execute

For example, to give read and write permissions to the owner, and read permissions to everyone else:

```bash
chmod 644 <file>
```
The first digit is for the owner, the second for the group, and the third for everyone else.








