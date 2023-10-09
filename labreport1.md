# Lab Report 1

## cd
1. cd
2. cd lecture1
3. cd messages

```
[user@sahara ~]$ cd
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ cd messages
[user@sahara ~/lecture1/messages]$
```
This command changes the directory of the workspace, so the directory changes from lecture1 to within messages file. There are no errors in these outputs. 

## ls
1. ls
2. ls lecture1
3. ls Hello.java

```
[user@sahara ~]$ ls
cse15llab1  Hello.java  lecture1
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
[user@sahara ~]$ ls Hello.java
Hello.java
```
For this one, I began with cd to take it back to the main directory and use ls to show what is within my home. Then I can continue to list what is in each file. There is no errors in these outputs. 

## cat
1. cat 
2. cat lecture1
3. cat Hello.java

```
[user@sahara ~]$ cat
[user@sahara ~]$ cat lecture1
cat: lecture1: Is a directory
[user@sahara ~]$ cat Hello.java
```

The cat command returns what is the command given or what is within the file. So just type cat makes the terminal wait for further text or adding lecture1 will define it as a directory for you. I believe their is no errors since the program is outputting the information it is being given. 
