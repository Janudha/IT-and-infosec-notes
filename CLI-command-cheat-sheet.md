# 🚀 System & Command Line Fundamentals

## 🐧 Linux
1. **`Whoami`**
2. **`echo`** - to get an output (eg: `echo "try hack me"` -> try hack me)
3. **`ls`** - list down
4. **`cd`** - change directory/folder
5. **`pwd`** - where am I
6. **`cat`** - show contents in a file
7. **`find`** - find the location of a file (eg: `find -name users.txt`)
8. **`grep`** - find specific contents inside a file (eg: `grep Williom users.txt`)
9. **`&`**
10. **`&&`**
11. **`>`**
12. **`>>`**
13. **`ssh`** - remote access of another device (eg: `ssh tryhackme@10.22.102.220`)
14. **flags & switches** - (eg flag: `ls -a`, eg switch: `ls --all`)
15. **`man`** - manual page (eg: `man ls`)
16. **`touch`** - create a file
17. **`mkdir`** - create a folder
18. **`rm`** - remove a file (To remove a folder: `rm -R yourfolder`)
19. **`cp`** - copy a file (eg: `cp note1 note2`)
20. **`mv`** - move a file or rename a file/folder (eg move: `mv note1 myfolder`) (eg rename: `mv note1 mynote`)
21. **`file`** - identifying the type of a file (eg: `file mynote`)
22. **`ls -lh`** - view permissions (eg: `rwxr--r-x` -> owner can read/write/execute, group can read only, others can execute only)
23. **`chmod`** - change permissions (eg: `chmod 721 tryhackme.txt` -> which means owner can rwx, group can w only, others can x only for tryhackme file)
24. **`su`** - switch between users (eg1- switch user: `su user2`) (eg2- switch and login: `su -l user2`)
25. **`/etc`** (a very important root folder)- a commonplace location to store system files that are used by our operating system (eg important files in this folder: 'sudeoers' file, 'shadow' file, 'passwd' file)
26. **`/root`** (a root folder)- this is the home directory for the "root" user
27. **`/tmp`** (a root folder)- "temporary"/ the tmp directory is volatile and is used to store data that is only needed to be accessed once or twice. Similar to the memory on our computer, once the computer is restarted, the contents of this folder are cleared out (for hackers; this is a good place to keep their enumeration scripts in target's computer)
28. **`/var`** (a root folder)- stores data that is frequently accessed or written by services or applications running on the system (eg files important files inside this folder: log files from running services and applications, databases, etc)
29. **`nano`** or **`vim`** - create files or edit files using text editors (eg: `nano myfile`)
30. **`wget`** - downloading files (eg: `wget https://assets.tryhackme.com/additional/linux-fundamentals/part3/myfile.txt`)
31. **`scp`** - send a file to another device via SSH (eg: `scp important.txt ubuntu@192.168.1.30:/home/ubuntu/transferred.txt`), take a file from another device via SSH (eg: `scp ubuntu@192.168.1.30:/home/ubuntu/documents.txt notes.txt`)
32. **`python3 -m  http.server`** - provides a lightweight and easy-to-use module called "HTTPServer", This module turns our computer into a quick and easy web server that we can use to serve our own files, where others can then be downloaded by another computing using commands such as curl and wget (eg download using this server: `wget http://10.67.151.243:8000/myfile`)
33. **`ps`** - provide a list of the running processes as our user's session (PID)
34. **`ps aux`** - To see the processes run by other users and those that don't run from a session
35. **`top`** -  gives you real-time statistics about the processes running on our system instead of a one-time view
36. **`kill`** - terminate processes (eg: `kill 1317` -> means terminate process under PID 1317)
37. **`systemctl`** - Start/Stop/Enable/Disable/Status of a process or service (eg: If you want to disable a service -> `systemctl disable myservice`)
38. **`ctrl + z`** or **`&`** - to background a process, so our terminal is no longer filled up with messages aka ongoing tasks (eg: `echo "Hi THM"` -> then press ctrl + z or `echo "Hi THM" &`)
39. **`fg`** - to foreground a process
40. **`apt`** - package management/ Apt contains a whole suite of tools that allows us to manage the packages and sources of our software, and to install or remove software at the same time (eg: `apt install sublime-text`),(eg: `apt remove sublime-text`),(eg: `apt update`)
41. **`/var/log`** - these files and folders contain logging information for applications and services running on your system. These services and logs are a great way in monitoring the health of our system and protecting it. Not only that, but the logs for services such as a web server contain information about every single request - allowing developers or administrators to diagnose performance issues or investigate an intruder's activity. For example, the two types of log files below that are of interest: access log, error log
42. **`crontab`** -  schedule a certain action or task to take place after the system has booted. (eg: running commands, backing up files, or launching our favorite programs on, such as Spotify or Google Chrome). Crontabs can be edited by using `crontab -e`, where we can select an editor (such as Nano) to edit our crontab. There are some great resources such as the online "Crontab Generator" that allows us to use a friendly application to generate our formatting for us!

---

## 🪟 Windows CLI
1. **`Set`** - to check your path from the command line
2. **`Ver`** - to determine the operating system (OS) version.
3. **`Systeminfo`** - to list various information about the system such as OS information, system details, processor and memory
4. **`help`** - Provides help information for a specific command
5. **`cls`** - Clears the Command Prompt screen
6. **`ipconfig`** - to see network information such as our IP address, subnet mask, and default gateway
7. **`ipconfig /all`** - for more information about your network configuration
8. **`ping target_name`** - to know we can reach the target and that the target can reach us
9. **`tracert target_name`** - traces the network route traversed to reach the target
10. **`nslookup example.com`** - looks up a host or domain and returns its IP address
11. **`netstat`** - displays current network connections and listening ports  (help page -> `netstat -h`)
12. **`cd`** - to display the current drive and directory
13. **`dir`** - view the child directories (`dir /a` - Displays hidden and system files as well. `dir /s` - Displays files in the current directory and all subdirectories)
14. **`tree`** - to visually represent the child directories and subdirectories
15. **`cd target_directory`** - to change any directory
16. **`cd ..`** - to go up one level
17. **`mkdir directory_name`** - to make directory
18. **`rmdir directory_name`** - To delete a directory
19. **`type`** - view text files
20. **`more`** - display enough text file contents to fill your terminal window
21. **`copy`** - allows you to copy files from one location to another
22. **`move`** - move files
23. **`del`** or **`erase`** - delete a file
24. **`*`** -  to refer multiple files (eg: `copy *.md C:\Markdown` will copy all files with the extension md to the directory C:\Markdown)
25. **`tasklist`** - list the running processes (You can check all available filters by displaying the help page using `tasklist /?` command)
26. **`taskkill /PID target_pid`** - to terminate a task (eg: `taskkill /PID 4567`)
27. **`chkdsk`** - checks the file system and disk volumes for errors and bad sectors
28. **`driverquery`** - displays a list of installed device driver.
29. **`sfc /scannow`** - scans system files for corruption and repairs them if possible
30. **`/?`** - to display help page of commands

---

## ⚙️ Windows Powershell
1. **`Get-command`**: To list all available cmdlets, functions, aliases, and scripts that can be executed in the current PowerShell session
2. **`Get-Command -CommandType "type"`**:  to filter the list of commands based on displayed property values (eg: if we want to display only the available commands of type “function”, we can use `Get-command -CommandType "Function"`)
3. **`Get-help`**: it provides detailed information about cmdlets, including usage, parameters, and examples (eg: `Get-Help Get-Date`)
4. **`Get-Alias`**: lists all aliases available
5. **`Find-Module`**: To search for modules (collections of cmdlets) in online repositories like the PowerShell Gallery if we want to download a cmdlet. We need an internet connection to fo this (eg: `Find-Module -Name "PowerShell*"`, If we don't know the exact name of the module -> `Cmdlet -Property "pattern*"`)
6. **`Install-Module`**: Once identified, the modules can be downloaded and installed from the repository (eg: `Install-Module -Name "PowerShellGet"`)
7. **`Get-ChildItem`**: to list the files and directories in a location
8. **`Set-Location`**: To navigate to a different directory (eg: `Set-Location`)
9. **`New-Item`**: To create an item in PowerShell. We will need to specify the path of the item and its type ,whether it is a file or a directory (eg: `New-Item -Path ".\captain-cabin\captain-wardrobe" -ItemType "Directory"`)
10. **`Remove-Item`**: to remove both directories and files (eg: `Remove-Item -Path ".\captain-cabin\captain-wardrobe\captain-boots.txt"`, `Remove-Item -Path ".\captain-cabin\captain-wardrobe"`)
11. **`Copy-Item`**: copy or move files and directories alike, using respectively Copy-Item (equivalent to copy) and Move-Item (equivalent to move). (eg: `Copy-Item -Path .\captain-cabin\captain-hat.txt -Destination .\captain-cabin\captain-hat2.txt`)
12. **`Get-Content`**: to read and display the contents of a file (eg: `Get-Content -Path ".\captain-hat.txt"`)
13. **`|`**: allows the output of one command to be used as the input for another (eg: `Get-ChildItem | Sort-Object Length` -> Here, Get-ChildItem retrieves the files (as objects), and the pipe (|) sends those file objects to Sort-Object, which then sorts them by their Length (size) property)
14. **`Where-Object`**: To filter objects based on specified conditions, returning only those that meet the criteria (eg: `Get-ChildItem | Where-Object -Property "Extension" -eq ".txt"` -> Where-Object filters the files by their Extension property, ensuring that only files with extensions equal (-eq) to .txt are listed)
15. **`Select-Object`**: used to select specific properties from objects or limit the number of objects returned (eg: `Get-ChildItem | Select-Object Name,Length`)
16. **`Select-String`**: searches for text patterns within files, similar to grep in Unix-based systems, used for finding specific content within log files or documents (eg: `Select-String -Path ".\captain-hat.txt" -Pattern "hat"`)
17. **`Get-ComputerInfo`**: retrieves comprehensive system information, including operating system information, hardware specifications, BIOS details, and more. provides a snapshot of the entire system configuration in a single command
18. **`Get-LocalUser`**: lists all the local user accounts on the system
19. **`Get-NetIPConfiguration`**: provides detailed information about the network interfaces on the system, including IP addresses, DNS servers, and gateway configurations
20. **`Get-NetIPAddress`**: show details for all IP addresses configured on the system, including those that are not currently active
21. **`Get-Process`**: provides a detailed view of all currently running processes, including CPU and memory usage, making it a powerful tool for monitoring and troubleshooting
22. **`Get-Service`**: retrieval of information about the status of services on the machine, such as which services are running, stopped, or paused
23. **`Get-NetTCPConnection`**: displays current TCP connections, giving insights into both local and remote endpoints
24. **`Get-FileHash`**: a useful cmdlet for generating file hashes, which is particularly valuable in incident response, threat hunting, and malware analysis, as it helps verify file integrity and detect potential tampering
25. **`Invoke-Command`**: essential cmdlet for executing commands on remote systems, making it fundamental for system administrators, security engineers and penetration testers (eg: `Get-Help Invoke-Command -examples`)
26. **`Get-Help`**:

---

## 💻 Linux Shell
1. **`echo $SHELL`**: To see which shell we are using
2. **`cat /etc/shells`**: list down the available shells in our Linux OS (The file /etc/shells contains all the installed shells on a Linux system)
3. **`zsh`**: To switch between shells, we can type the shell name which we want that is present on our OS
4. **`chsh -s /usr/bin/zsh`**:  to permanently change our default shell
5. **`history`**: to see the entered commands history
6. **`.sh`**: to create a shell script(like bash script) file using any text editor (eg: `nano first_script.sh`)
7. **`#!/bin/bash`**: Every script should start from shebang. Shebang is a combination of some characters that are added at the beginning of a script (starting with #! followed by the name of the interpreter)
8. **`chmod +x first_script.sh`**: To give permissions to execute the script
9. **`./`**: use this before the script name to execute it
10. **Variables**: stores a value inside it (Instead of memorizing and writing a value repeatedly, you can store them in a variable and use the variable name wherever you need it) eg:- A string: "Hey, what’s your name?” This is done by echo command. The second line of the script contains the code 'read name'. 'read' is used to take input from the user, and 'name' is the variable in which the input would be stored. The last line uses echo to display the welcome line for the user, along with its name stored in the variable. ➡️ 
    ```bash
    #!/bin/bash  
    echo "Hey, what’s your name?"  
    read name  
    echo "Welcome, $name"
    ```
11. **Loops**: let’s write a loop that will display all numbers starting from 1 to 10 on the screen (The first line has the variable i that will iterate from 1 to 10 and execute the below code every time. do indicates the start of the loop code, and done indicates the end. In between them, the code we want to execute in the loop is to be written. The for loop will take each number in the brackets and assign it to the variable i in each iteration. The echo $i will display this variable’s value every iteration. ➡️ 
    ```bash
    #!/bin/bash  
    for i in {1..10};  
    do  
    echo $i  
    done
    ```
12. **Conditional Statements**: they help us execute a specific code only when a condition is satisfied; otherwise, you can execute another code. (eg: you want it to be shown to only some users, only to the high-authority user. You will create a conditional statement that will first ask the user their name, and if that name matches the high authority user’s name, it will display the secret. ➡️ 
    ```bash
    #!/bin/bash  
    echo "Please enter your name first:"  
    read name  
    if [ "$name" = "Stewart" ]; then  
    echo "Welcome Stewart! Here is the secret: THM_Script"  
    else  
    echo "Sorry! You are not authorized to access the secret."  
    fi
    ```
13. **Comments**: A comment is a sentence that we write in our code just for the sake of our understanding. It is written with a # sign followed by a space and the sentence you need to write. (eg: `# Asking the user to enter a value.  echo "Please enter your name first:"`)
14. **The Locker Script**: you can make a locker script to lock something and verify a user before opening it