## Basic Commands

Display Linux system information

```bash 
#uname -a
``` 

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/uname-a.PNG)

Display kernel release information

```bash 
#uname -r
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/uname-r.PNG)

Show which version of redhat installed

```bash 
# cat /etc/redhat-release
```
![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/release.PNG)

Show how long the system has been running + load

```bash 
# uptime
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/uptime.PNG)

Show system host name

```bash 
# hostname
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/hostname.PNG)

Display the IP addresses of the host

```bash 
# hostname -I
```
![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/hostname-i.PNG)

Show system reboot history

```bash 
# last reboot
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/lastreboot.PNG)

Show the current date and time

```bash 
# date
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/date.PNG)

Show this month's calendar

```bash 
# cal
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cal.PNG)

You can see your previously run command by executing 'history' command

```bash
# history
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/history.PNG)

Display who is online

```bash 
# w
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/w.PNG)

Who you are logged in as

```bash 
# whoami
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/whoami.PNG)


## Navigating Path

The pwd command displays the full path name of the current location, which helps determine appropriate syntax for reaching files using relative path names. 

```bash
# pwd
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/pwd.PNG)

The ls command lists directory contents for the specified directory, or if no directory is given for the current directory. as in if I enter "ls /etc" it will display the files and directories under /etc directory 

```bash 
# ls /etc
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/lsetc.PNG)

Use the cd command to change directories. As example if you run "cd /etc" it will change the directory to /etc

```bash
# cd /etc
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cdetc.png)

Use the cd command to change working directory to logged in user home directory. "cd" and "cd ~" both command will change the working directory to the logged in users home dorectoy.

```bash
# cd 
# cd ~
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cd.png)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cdhome.png)

use the cd command with .. to change the working directory to parent directory. It works like the the up button of windows explorer. By default every users home directory situated in /home directory so if we execute the command "cd .." from any users directory it will take you the the directory /home.

```bash
# cd ..
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cdup.png)

use the cd command with - to change the working or current directory to previous working directory. This means if I change the directory to /etc from /home and then I executed "cd -" it will take back you to /home

```bash
# cd -
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cdprev.PNG)


The ls command has multiple options for displaying attribute on files. The most common and useful are –l (long listing format), -a (all files includes hidden files) and –R (recursive)

```bash
# ls -l
# ls -la
# ls -R
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/lsl.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/lsla.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/lpr.PNG)
### File and Directory Management
use mkdir command to create directory

```bash
# mkdir dir
# ls
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/mkdir.PNG)

The mkdir command creates one or more directories or subdirectories, generating errors if the filename already exists or when attempting to create a directory in a parent directory that doesn’t exist. The –p parent option creates missing parent directories for the requested destination.

```bash
# mkdir dir2/subdir2 
# mkdir dir2/subdir2 -p
#ls
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/mkdirerr.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/mkdirp.PNG)

use touch command to create directory

```bash
# touch file1
# ls
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/touch.PNG)

to create multiple command with command

```bash
# touch file1 file2 file3
# ls
# touch filename{1..5}
# ls
# touch file.txt /tmp/file.txt
# ls
# ls /tmp
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/touchm.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/touchml.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/touchmdl.PNG)

The cp command copies one or more files to become new, independent files. Syntax allows copying an existing file to a new file in the current or another directory, or copying multiple files into another directory. In any destination, new file names must be unique. If the new file name is not unique, the copy command will overwrite the existing file. When copying multiple files with one command, the last argument must be a directory.

```bash
# ls
# cp file1 myfile.txt
# ls
# ls /tmp
# cp file1 /tmp/
# ls /tmp
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cp.png)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cpdl.PNG)

The mv command renames files in the same directory, or relocates files to a new directory. File contents remain unchanged. Files moved to a different file system require creating a new file by copying the source file, then deleting the source file.

```bash
# ls
# mv file2 file2.txt
# ls
# ls
# mv file3 /tmp/
# ls
# ls /tmp
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/mv.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/mvdl.PNG)

Default syntax for rm deletes files, but not directories. Deleting a directory, and potentially many subdirectories and files bellow it, require the –r recursive option. Using -i will interactively prompt for each deletion. This is essentially the opposite of –f which will force the deletion without prompting the user. There is no command-line undelete feature, nor a trash bin from which to restore.

```bash
# ls
# rm filename1
# ls
# ls
# rm -rf dir2
# ls
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/rm.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/rmd.PNG)

The rmdir directoris only if empty. Removed directories cannot be undelete.

```bash
# ls
# rmdir dir
# ls
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/rmdir.PNG)

### Read a file in Linux

To read a file one of the most popular command is "cat". cat followed by by the file name or path will display the file content in your shell

```bash
# cat myfile
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/cat.PNG)

To read a file in a reverse direction we can use "tac" command

```bash
# tac myfile
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/tac.PNG)

"head" is a command to read first 10 lines of a file you can specify the line number by using -n command followed by the desired line number

```bash
# head /etc/passwd
# head -n 3 /etc/passwd
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/head.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/headn.PNG)

"tail" is a command to read last 10 lines of a file you can specify the line number by using -n command followed by the desired line number. and we can use -f option to follow the file continiously, which is very useful to read logs 

```bash
# tail /etc/passwd
# tail -n 3 /etc/passwd
# tail -f 
```

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/tail.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/tailn.PNG)

![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/tailf.PNG)


"head" is a command which is used for reading big file can't read with single screen and have to scroll down. We can scroll the file downwards by pressing "Enter" or "Space" button. And it will take you out from the file when you scroll it down all the way to the end of the file.

```bash
# more /var/log/messages
```
![alt text](https://github.com/shiblijoy/shiblijoy/blob/master/more.PNG)

"less" is a command which is used for reading big file can't read with single screen and have to scroll up and down. We can scroll the file upwards or downwards by pressing "Up Arrow" or "Down Arrow" button. And you have to press the button "q" to get out from the file.

```bash
# less /var/log/messages
```
