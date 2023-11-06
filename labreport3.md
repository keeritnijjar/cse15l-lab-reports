# Lab Report 3

Find Command

1. find -name "filename" 
   - this command will search the home directory for a specific file name
   - Examples:
```
find -name lib
./lib
```
```
find -name technical
./technical
```
These lines show the input and the output, returns the file path in the directory 

2. find ./[filepath]
   - This command returns all the files and directories in the directory listed
   - Examples:

```
find ./lib
./lib
./lib/hamcrest-core-1.3.jar
./lib/junit-4.13.2.jar
```
```
find ./technical
./technical
./technical/911report
./technical/911report/chapter-13.3.txt
./technical/911report/chapter-13.2.txt
./technical/911report/chapter-6.txt
./technical/911report/chapter-5.txt
...
```
This allowed me to see what files are in each folder for lib or technical

3. find ~ -type f(d)
   - this allows to find file, directories by type
   - Examples:
  
```
find ~ -type f
/home/docsearch/technical/911report/chapter-13.3.txt
/home/docsearch/technical/911report/chapter-13.2.txt
/home/docsearch/technical/911report/chapter-6.txt
/home/docsearch/technical/911report/chapter-5.txt
... 
```
```
find ~ -type d
/home/docsearch/technical
/home/docsearch/technical/911report
/home/docsearch/technical/biomed
/home/docsearch/lib
/home/docsearch/.git
/home/docsearch/.git/logs
/home/docsearch/.git/logs/refs
...
```
Using this command shows the list the files in the directory, for the second example I used type d which finds the directories

4. find ~ -type f(d) -empty
   - this allows to find files, directories that are empty
   - Examples:
  
```
find ~ -type f -empty
(did not find empty file in docsearch)
```
 ```
find ~ -type d -empty
/home/docsearch/.git/refs/tags
/home/docsearch/.git/branches
/home/docsearch/.git/objects/info
```  
Using this for type f did not return anything but using it for type d returned empty directories, I noticed that they didn't show up for type f but do for type d
