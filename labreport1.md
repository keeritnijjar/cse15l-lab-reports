# Lab Report 1

## cd
1. cd
2. cd lecture1
3. cd Hello.java

```
[user@sahara ~]$ cd
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ cd Hello.java
bash: cd: Hello.java: Not a directory
```
1. Working Directory: Home, Description: This command changes the directory of the workspace but since I didn't choose a directory it doesn't assign any directory just stays at the home directory, Error: no error 
2. Working Directory: lecture1, Description: I assigned the directory to be within lecture1, Error: no error since there is a proper directory
3. Working Directory: still lecture1 from my previously assigned directory, Description: I am trying to change the directory to a file, Error: This will show an error since Hello.java is not a directory

## ls
1. ls
2. ls lecture1
3. ls Hello.java

```
[user@sahara ~]$ ls
cse15llab1  Hello.java  lecture1
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
[user@sahara ~]$ ls messages
ls: cannot access 'messages': No such file or directory
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ ls messages
af.txt  en-us.txt  es-mx.txt  zh-cn.txt
[user@sahara ~/lecture1]$ 
```
For this one, I began with cd to take it back to the main directory and use ls to show what is within my home. Then I can continue to list what is in each file.
1. Working Directory: Home, Description: used ls to see what is in the home directory, Error: no error since it shows the result correctly
2. Working Directory: Home, Description: used ls to see what is in the lecture1 directory, Error: no error since it shows the result correctly
3. Working Directory: Home, Description: I tried to use ls to list the files inside the messages directory but since the directory wasn't assigned it couldn't access them so I changed the working directory to lecture1 and I was able to list all files in messages, Error: no errot just need to assign working directory

## cat
1. cat 
2. cat lecture1
3. cat Hello.java

```
[user@sahara ~]$ cat
hi me
hi me
^C
[user@sahara ~]$ cat lecture1
cat: lecture1: Is a directory
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ cat Hello.java
import java.io.IOException;
import java.nio.charset.StandardCharsets;
import java.nio.file.Files;
import java.nio.file.Path;

public class Hello {
  public static void main(String[] args) throws IOException {
    String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
    System.out.println(content);
  }
```

1. Working Directory: Home, Description: Using just cat will result in a loop where the terminal will return whatever you type back and then I exited to get out of it, Error: no error just no additional thing to read 
2. Working Directory: Home, Description: cat lecture1 tells us what lecture1 is so it is a directory, Error: no error since its correct
3. Working Directory: lecture1, Description: After changing the working directory to lecture1, if I cat Hello.java it returns every line of code in the file, Error: No error since it returned it's decription 
