# Lab Report 3 

## Part 1
Looking at teh command find. The 4 intresting command line options to use these commands are: 
-name , -type, -perm, and -user. Following the general syntax of fine, which is 
`
find [options] [path] [expression]
`
.

---
Looking at -name, this command prompt tells the find command to search for the file by its name
and what ever it is followed by that is the name that the find command will search for.

For exmaple, from the files and directories from ./technical:
```
find ./technical -name "reports*"
```
This will find all the files in the **./technical** directory that starts the name reports. This is
really useful when searching through a huge directory for files that starts with a certain name.

```
find ./technical -name "*"
```
This would fina all the fiels in the **./technical** with out any type of specification.
The point of htis command prompt isto search for all the files in the **./technical** directory 
This is good to retreieve all the iteam in the directory.

---
Looking at -type, this command is normally used to search for specific file type. There is an option that follows it to specify the file type:
* d: directory
* f: file

For example, form the file and directory from ./technical
```
find ./technical -type f
```
This finds all the files that are in the **./technical** directory. This is really helpful when looking for regular files, really nice when the user wants to look for a specific file.

```
find ./technical -type f -name "*.txt"
```
This command finds all the text files that are in teh **./technical** directory. This command prompt also uses *-name "*.*txt"*. Therefore this whole commandsearches through the directoy fore files that are text files. This is really helpful when there are a large amount of files and want to search for a specific file type.

---
Looking at



