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
