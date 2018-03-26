# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

>> 1. show current working directory path: `pwd`
>> 2. creating a directory: `mkdir`
>> 3. deleting a directory: `rm`
>> 4. creating a file using: `touch` command: `touch`
>> 5. deleting a file: `rm -f`
>> 6. renaming a file: `mv old_name new_name`
>> 7. listing hidden files: `ls .?*`
>> 8. copying a file from one directory to another: `cp from_directory to_directory`
>> 9. listing long files including hidden files: `ls -al`
>> 0. moving files from one directory to another: `mv from directory to_directory`

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

>> + `ls`: lists all files in the directory
>> + `ls -a`: displays all files
>> + `ls -l`: displays the long format listing
>> + `ls -lh`: shows sizes in human readable format
>> + `ls -lah`: lists all humen readables
>> + `ls -t`: displays newest files first (based on timestamp)
>> + `ls -Glp`: displays directories with / in a long listing, don't print group names

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

>> + `-b`: Displays nonprinting characters in octal.
>> + `-c`: Displays files by file timestamp.
>> + `-d`: Displays only directories.
>> + `-f`: Interprets each name as a directory, not a file.
>> + `-g`: Displays the long format listing, but exclude the owner name.

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

>> It converts input from standard input into arguments to a command. [wikipedia](https://en.wikipedia.org/wiki/Xargs 'xargs')

>> `$ echo "splitXsplitXsplitXsplit" | gxargs -d X -n 2`

>> `split split`

>> `split split`

>> This example comes from _Linux Shell Scripting Cookbook - 3rd Edition_,  
>> Using `gxargs` instead of `xargs` because mac os x doesn't have `-d` option to change the input delimiter.  
>> `gxargs` requires installation of `findutils`. 

 

