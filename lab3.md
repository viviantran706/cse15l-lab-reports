# Lab Report 3 

## Part 1
Looking at teh command find. The 4 intresting command line options to use these commands are: 
-name , -type, -size, and -regex. Following the general syntax of fine, which is 
`
find [options] [path] [expression]
`
.

---
Looking at -name, this command prompt tells the find command to search for the file by its nameand what ever it is followed by that is the name that the find command will search for.

For exmaple, from the files and directories from **./technical**:
```
find ./technical -name "reports*"
```
```
Output:
./technical/reportsHousing.txt
./technical/reports/
./technical/reportFromOneYearAgo.pdf
```
This will find all the files in the **./technical** directory that starts the name reports. This is
really useful when searching through a huge directory for files that starts with a certain name.

```
find ./technical -name "*"
```
```
Output:
./technical/directory1/file1.txt
./technical/document.pdf
./technical/image.jpg
./technical/file.txt
```

This would fina all the fiels in the **./technical** with out any type of specification.
The point of htis command prompt isto search for all the files in the **./technical** directory. This is good to retreieve all the iteam in the directory.

Website used:[Link](http://a.com)

---
Looking at -type, this command is normally used to search for specific file type. There is an option that follows it to specify the file type:
* d: directory
* f: file

For example, form the file and directory from **./technical**
```
find ./technical -type f
```
```
Output:
./technical/document.pdf
./technical/image.jpg
./technical/file.txt
```

This finds all the files that are in the **./technical** directory. This is really helpful when looking for regular files, really nice when the user wants to look for a specific file.

```
find ./technical -type f -name "*.txt"*
```
```
Outputs:
./technical/files1.txt
./technical/files2.txt
./technical/files3.txt
```

This command finds all the text files that are in teh **./technical** directory. This command prompt also uses *-name "*.*txt"*. Therefore this whole commandsearches through the directoy fore files that are text files. This is really helpful when there are a large amount of files and want to search for a specific file type.

Citation
---
Looking at -size, this command is normally used to search for a sepcific file based on the file size.

For example, from the directory **./techical**:

```
find ./technical -type f -size +10K
```
```
Outputs:
./technical/file2_largerThan10K
./technical/file3_largerThan10K
./technical/file1_largerThan10K
```

For this command, the find commands will search all files in the **./technical** directory that are 10 kilobyte or larger. This command is useful if you are searching for managing a disk space, that would need to find anything that needs to be deleted.

```
find ./technical -type d -size +1M
```
```
Outputs:
./technical/larger_then1M_directory1
./technical/larger_then1M_directory2
./technical/larger_then1M_directory3
```

This command , will find all the directoires in the **./technical** directory that is 1 megabyte or larger. This helps of the user wants to search for directory based on teh size. Which is useful if you do want to look for a certian directory with these criterias.

---
Looking for -regex, is a war to search for files and directories that have regular expressional patterns.
```
find ./technical -type f -regex "*.*/file[0-8]"
```
```
Outputs:
./technical/file2
./technical/file3
./techical/file8
```
This command,  will find all the files that starts with file followed buy a number 0-8 with in the directory **./technical**. This command is useful when you want to find files that starts with file and a number. This would held locate them based on thier patterns

```
find ./technical -type d regex "*.*/playing[[:alpha:]]+"
```
```
Outputs:
./technical/playingCrazy
./technical/playingInClass
./technicalplayingWithFriends
```
This command, will find all the directoriees that starts with "playing" followed by a word. This command is useful because when trying to search for a directory in the directory ** ./technical** that starts with playing and one more more alphabetic characters. This makes it easier to find directories that fillow a patteren and if it needs to be located.
