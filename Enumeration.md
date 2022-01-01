## Enumeration

- hostname : prints the host name of the machine
    
- uname -a : prints the kernel version
    
- /proc/version : contains the OS info
    
- /etc/issue : contains info about OS
    
- ps -A : View all running processes
    
- ps axjf : View process tree
    
- env : command will show environmental variables.
    
- sudo -l : command can be used to list all commands your user can run using sudo
    
- ls -al : lists all files inside the directory
    
- id : command will provide a general overview of the user’s privilege level and group memberships
    
- /etc/passwd : contains info about users on the system
    
- history : command can give us some idea about the target system and, albeit rarely, have stored information such as passwords or usernames.


    
- Find Command


	- find . -name flag1.txt: find the file named “flag1.txt” in the current directory 
	- find /home -name flag1.txt: find the file names “flag1.txt” in the /home directory
	- find / -type d -name config: find the directory named config under “/”
	-  find / -type f -perm 0777: find files with the 777 permissions (files readable, writable, and executable by all users)
	-  find / -perm a=x: find executable files
	-  find /home -user frank: find all files for user “frank” under “/home”
	-   find / -mtime 10: find files that were modified in the last 10 days
	-   find / -atime 10: find files that were accessed in the last 10 day
	-   find / -cmin -60: find files changed within the last hour (60 minutes)
	-   find / -amin -60: find files accesses within the last hour (60 minutes)
	-   find / -size 50M: find files with a 50 MB size
	- 	find / -writable -type d 2>/dev/null : Find world-writeable folders
    - 	find / -perm -222 -type d 2>/dev/null: Find world-writeable folders
    -	find / -perm -o w -type d 2>/dev/null: Find world-writeable folders
    -	find / -perm -o x -type d 2>/dev/null : Find world-executable folders
    -	find / -perm -u=s -type f 2>/dev/null: Find files with the SUID bit, which allows us to run the file with a higher privilege level than the current user. (imp)
	### devopemnet language
    -	find / -name perl*
    -	find / -name python*
    -	find / -name gcc*
- Capabalities ``getcap`` to list enabled capabilities
- Cronjobs can be found under ``/etc/crontab`` can run certain scripts as root these scripts can sometimes be editable by unpriveleged users
- Changing the ``$PATH`` variable

 
    
    
    
   
    
    
   
    
   
    
    