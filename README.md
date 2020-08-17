## Basic Commands

Display Linux system information

```bash 
#uname -a
```
Display kernel release information

```bash 
#uname -r
```


Show which version of redhat installed

```bash 
#cat /etc/redhat-release
```

Show how long the system has been running + load

```bash 
#uptime
```

Show system host name

```bash 
#hostname
```

Display the IP addresses of the host

```bash 
#hostname -I
```

Show system reboot history

```bash 
#last reboot
```

Show the current date and time

```bash 
#date
```

Show this month's calendar

```bash 
#cal
```

Display who is online

```bash 
#w
```

Who you are logged in as

```bash 
#whoami
```


## Navigating Path

The pwd command displays the full path name of the current location, which helps determine appropriate syntax for reaching files using relative path names. 

```bash
#pwd
```

The ls command lists directory contents for the specified directory, or if no directory is given for the current directory.

```bash 
# ls
```

Use the cd command to change directories.

```bash
# cd /etc
```

The ls command has multiple options for displaying attribute on files. The most common and useful are –l (long listing format), -a (all files includes hidden files) and –R (recursive)

```bash
# ls-l
# ls -la
# ls -R
```
### File and Directory Management
use mkdir command to create directory

```bash
# mkdir dir/subdir
```

The mkdir command creates one or more directories or subdirectories, generating errors if the filename already exists or when attempting to create a directory in a parent directory that doesn’t exist. The –p parent option creates missing parent directories for the requested destination.

```bash
# mkdir dir2/subdir2 -p
```

use touch command to create directory

```bash
# touch file1
```

to create multiple command with command

```bash
# touch file1 file2 file3
# touch filename{1..5}
# touch file.txt /tmp/file.txt
```

The cp command copies one or more files to become new, independent files. Syntax allows copying an existing file to a new file in the current or another directory, or copying multiple files into another directory. In any destination, new file names must be unique. If the new file name is not unique, the copy command will overwrite the existing file. When copying multiple files with one command, the last argument must be a directory.

```bash
# cp file1 file1.txt
#cp file /tmp/
```

The mv command renames files in the same directory, or relocates files to a new directory. File contents remain unchanged. Files moved to a different file system require creating a new file by copying the source file, then deleting the source file.

```bash
# mv file2 file2.txt
# mv file2 /tmp/
```

Default syntax for rm deletes files, but not directories. Deleting a directory, and potentially many subdirectories and files bellow it, require the –r recursive option. Using -i will interactively prompt for each deletion. This is essentially the opposite of –f which will force the deletion without prompting the user. There is no command-line undelete feature, nor a trash bin from which to restore.

```bash
# rm file3
# rm -rf dir2
```

The rmdir directoris only if empty . Removed directories cannot be undelete.

```bash
# rmdir dir
```

