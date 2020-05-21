## GIT COMMANDS


### File Commands

#### Creating New Directory
```mkdir``` command is used to create new dircetory
```
$ mkdir MyProj

```
This will create the MyProj in your working directory

#### Checking Current Directory
```pwd``` command is used to check current directory
```
$ pwd
c\user\
```
Suppose You were in c:/user initially

#### Changing Directory
```cd``` command is used to change directory to the directory present in the current directory
```
$ cd MyProj
```
Now current directory is MyProj, which can be checked by pwd
```
$ pwd
c\user\MyProj
```

#### Shifting Back to previous directory
```cd ..``` command  returns to the previous directory
```
$ cd ..
$ pwd
c\user\
```
 ```cd ../.. ``` command returns to two previous directory (if exist) 

#### Creating New File
```echo > abcd.xyz ``` command creates a file named abcd with extension .xyz
```
$ echo > index.html
```
This will create and html file with name index

#### Creating new file with some data
``` echo "<data>" > abcd.xyz ``` creates a file named abcd.xyz with some data in it. 
```
$ echo "Hello World" > sample.txt
```
 This will create a sample.txt file with "Hello World" or overwrite "Hello World" to it, if Sample.txt already exists

#### Reading File
```cat``` command reads out the data of the file 
```
$ cat sample.txt
Hello World
```
It preserves all white spaces on execution

#### Deleting file or directory
```rm <filename.extention>``` removes the file and ```rmdir <directort name>``` removes the directory 
```
$ rm index.html
```
This removes the index.html file
```
$ rmdir MyProj2
```
This command will delete the MyProj2 folder in the working directory if present or it raises File Not Found Error
> Note : If you try to remove directory using ```rm``` command , then it will raise error saying ```Can't delete <DIR_NAME>: Is a directory``` .
However ```rm``` command can be used to delete directories using ```rm -r <DIR_NAME>``` command.

#### Renaming or Moving a file or directory
```mv``` command is used to rename and move a file
#### syntax
1.  ```mv <file1.extension> <file2.extension>``` : It changes the name of file1 to file2
2.  ```mv <file1.extension> <DIR_NAME>``` : It moves file to directory, if it exists else name changes to dir name
3. ```mv <DIR1> <DIR2>``` : It renames the Directory1 to Directory2, provided there is no Directory with the same name as Directory2
4. ```mv <DIR1> <DIR2>``` : It moves the Directory1 to the Directory2, if it is already present in the main folder.

> It can be said that ```mv A B``` changes A to B, if B is not already in the folder else moves A inside B.
If A and B both are files then A's name is changed to B and original B is deleted (Point to be Noted).


#### Copying File
```cp file1 destination``` command copies the file1 to destination 
```
$ cp sample.txt MyProj2
```
You cant copy files to the same directory

#### Copying Directory
```cp -r DIR_NAME destination``` command copies the directory to destination 
```
$ cp MyProj2 MyProj3
```
You cant directory to the same directory

#### Copying All
```cp -r . destination``` copies all the files and directories in the current directory to the destination folder
##### Note : The same folder will not be copied to itself.

#### Clearing Prompt/Terminal/Bash
```clear``` command clear the screen and gives you a fresh screen 
```
$ clear
```

##### Tip : Use above arrow button to access earlier typed commands.