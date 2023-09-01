# Project1 
## Working with the Linux Commands

### Commands
#### 1. sudo Command:
> The sudo command allows you to execute root/administrative tasks.
>* Here's the general syntax
sudo (command e.g apt upgrade)

sudo apt upgrade

#### `Command Result`

<img width="812" alt="Screenshot 2023-08-23 at 08 31 36" src="https://github.com/tundek/DevOps_Projects/assets/15998669/d7d90fec-d5d5-422a-bd8c-cdb09d4ba369">

#### 2. pwd Command:
>This command shows your present working directory (pwd). It can also be used along side with tag to extend it's function
>* Syntax is pwd [option]

#### `Command Result`

<img width="619" alt="Screenshot 2023-08-23 at 08 35 18" src="https://github.com/tundek/DevOps_Projects/assets/15998669/58db5187-6ba5-4174-8cd2-4f2e0527944f">

#### 3. cd Command:
>This command is used to navigate the different folders/directories on your server.
>For example, opening and/or closing folder(s) on GUI
>* Syntax is cd [directory/folder name]
Navigates to the specified directory name

Another use case(s) could be 
>* cd - (Takes you to the previous working directory)
>* cd  (Takes you to the home directory)
>* cd .. (Takes you one directory less)

#### `Command Result`

<img width="727" alt="Screenshot 2023-08-23 at 08 58 03" src="https://github.com/tundek/DevOps_Projects/assets/15998669/543725ad-9d45-45ff-8e46-432c473fb38c">

#### 4. ls Command:
>This command lists all files and directories in the current working directory. Hope it makes sense, Lol
The ls command can be used with other flags to make it more powerful
>* ls -l (List files and directories in the current working directory)
>* ls -a (List all files/folders including hidden files)
>* ls -R (List all the files in subdirectories)
>* ls -lh (Shows all the files and their sizes)
>* ls -la (Lists all the files/folders including hidden files/folders and their properties (including file permissions, who has access to what))

#### `Command Result`

<img width="911" alt="Screenshot 2023-08-23 at 09 09 23" src="https://github.com/tundek/DevOps_Projects/assets/15998669/253b03a2-8f62-415e-bc49-d5a70661b6d6">

#### 5. cat Command:
>The cat command is used to display the content of a file

Syntax > cat [filename]

>Can also be used to merge files 

cat filename1.txt filename2.txt > filename3.txt

>copies the content of filename1 merges with filename2 and outputs the result in another file, filename3.txt

#### `Command Result`

<img width="734" alt="Screenshot 2023-08-23 at 09 25 33" src="https://github.com/tundek/DevOps_Projects/assets/15998669/4ef11620-737a-4722-8b9f-9bbfc0fb4401">

#### 6. cp Command:
>cp command is used to copy a file or folder from one location to another, keeping the original copy

Example snippet: cp sample DevOps/  >> Makes a copy of the sample file from the current directory to DevOps directory

We can also copy multiple files from source to destination
Code sample: cp filename1.txt filename2.txt filename3.txt /home/username/Documents

To copy an entire directory use the flag -R along side the cp command.

```
cp -R /home/username/Documents /home/username/Documents_backup
```

#### `Command Result`
<img width="705" alt="Screenshot 2023-08-24 at 08 01 32" src="https://github.com/tundek/DevOps_Projects/assets/15998669/4bbe9d77-e7b5-478a-a87f-bd116e78fe2c">

#### 7. mv Command:
>cp command is used to move a file or directory from one location to another, WIthout keeping the original copy, from the name move.
>Additionally it can also be used to rename files/directories

```
mv sample.txt new_file
```
#### `Command Result`
<img width="698" alt="Screenshot 2023-08-24 at 08 46 15" src="https://github.com/tundek/DevOps_Projects/assets/15998669/0924f9da-b194-447b-9f19-fabb007520ad">

<img width="770" alt="Screenshot 2023-08-24 at 08 42 36" src="https://github.com/tundek/DevOps_Projects/assets/15998669/99e5b1fb-57c9-4b83-b2ad-c6526b33558b">

#### `Command Result` Used to rename file 
<img width="723" alt="Screenshot 2023-08-24 at 08 29 59" src="https://github.com/tundek/DevOps_Projects/assets/15998669/696c48a3-e892-42e0-b61c-8273730f41e1">


#### 8. mkdir Command:
>This command is used to create a new directory.


mkdir new_folder

mkdir folder/sub_folder

mkdir Music/Songs (This creates a directory Songs inside of directory Music)

#### `Command Result`

<img width="730" alt="Screenshot 2023-08-24 at 08 48 59" src="https://github.com/tundek/DevOps_Projects/assets/15998669/928048d1-535b-44d8-803f-4b38adb37281">


#### 9. rmdir Command:
>This command is used to permanently delete an empty subdirectory.

 ```
  rmdir new_foler/sub_folder
```

<img width="779" alt="Screenshot 2023-08-24 at 09 04 05" src="https://github.com/tundek/DevOps_Projects/assets/15998669/f0c27d55-aef6-4434-bc5b-41250f306573">

>The above command deletes(removes) the sub_folder

>If the command is used with a flag -p it removes both the new_folder and it's subfolder

```
  rmdir -p new_foler/sub_folder
```

<img width="876" alt="Screenshot 2023-08-24 at 09 13 52" src="https://github.com/tundek/DevOps_Projects/assets/15998669/393fbf6c-191d-4683-a8ac-2d88733974dc">


#### 10. rm Command:
>This command is used to delete files within a directory

Syntax: rm filename.  We can also combine with the flag, -R to delete the files and folder recursively. (Removes all files and directories)

To remove multiple files, 

rm filename filename2 filename3

<img width="632" alt="Screenshot 2023-08-24 at 09 23 41" src="https://github.com/tundek/DevOps_Projects/assets/15998669/be3bf355-182b-455e-8c1b-c5a0915fcd38">


#### 11. touch Command:
>This command is used to create an empty file

Example touch new_file

<img width="622" alt="Screenshot 2023-08-24 at 09 28 53" src="https://github.com/tundek/DevOps_Projects/assets/15998669/f06dda8a-3605-42db-b83c-ef14462c591d">


#### 12. locate Command:
>This command is used to find files

Example locate -i new_file

<img width="723" alt="Screenshot 2023-09-01 at 18 04 41" src="https://github.com/tundek/DevOps_Projects/assets/15998669/c5ea0c19-ba54-474f-a3b9-e53ccd77c63b">


#### 13. find Command:
>This command is similar to the locate cmd  to find files

Syntax: find [option] [path] [expression]

<img width="794" alt="Screenshot 2023-09-01 at 18 00 49" src="https://github.com/tundek/DevOps_Projects/assets/15998669/895e60a5-c159-4950-8b62-fea273b50eb5">



#### 14. grep Command:
>This command is used to find a keyword in a file. It searches through all the text in a specific file.
>
Syntax: grep search_word sample.txt (Searches the word 'search_word' in the file sample.txt

#### `Command Result`

<img width="666" alt="Screenshot 2023-08-25 at 07 44 56" src="https://github.com/tundek/DevOps_Projects/assets/15998669/b20a7c3b-0efb-4fc0-8ace-6beabf2781ea">

#### 15. df Command:
> We can use the df command to report the system disk space usage
Syntax:
```
   df [options] [file]
```
Use the -h flag for human readable format

### `Command Result`
<img width="1280" alt="Screenshot 2023-08-25 at 07 54 13" src="https://github.com/tundek/DevOps_Projects/assets/15998669/7ad7920a-1cc1-48c6-a4e3-16c286e68c66">


#### 16. df Command:
> We can use the df command to check how much space a file or directory takes up

> Syntax: du [file_name]/[directory_name]

#### `Output`

<img width="521" alt="Screenshot 2023-08-25 at 08 03 53" src="https://github.com/tundek/DevOps_Projects/assets/15998669/6d99c4f7-b0b1-4a18-b37c-c67709d84b6e">


#### 17. head Command:
> The head command is used to display the first 10 lines of a text file/document
> Syntax: head [file_name]


#### 18. tail Command:
> The tail command is used to display the last 10 lines of a text file/document
> Syntax: tail [file_name]


#### 19. diff Command:
> The diff command (different) is used to compare the contents of two files and displays the part that do not match.
> Syntax: diff [option] [file_name1] [file_name2]

#### `Output`

<img width="819" alt="Screenshot 2023-08-25 at 08 17 49" src="https://github.com/tundek/DevOps_Projects/assets/15998669/76dba3c0-2a8a-4e3e-9b08-26089012619a">

#### 20. tar Command:
> The tar command archives multiple files into TAR file.
> Syntax: tar [options] [archive_file] [file or directory to be achived]


# File Permissions and Ownership

#### 21. chmod Command:
> The chmos command is a commom command used to modify a file or directory's read, write and execute permissions.
Three user classes exists in Linux
> Owner
> group members
> others
>

```
  Syntax: chmod [options] [permission] [file_name] 
```

#### `Output`

<img width="752" alt="Screenshot 2023-08-25 at 08 42 22" src="https://github.com/tundek/DevOps_Projects/assets/15998669/de3aa6fa-649f-4071-9ebd-a06d75912ff1">

#### 22. chown Command:
> The chmos command is used to change the ownership of a file/directory or symbolic link to a specified username.
Three user classes exists in Linux
> Syntax: chown [option] owner[:group] file(s)
```
chown linuxuser2 filename.txt
```

#### 23. Jobs Command:
> A job is process started by the shell. The job command will display all the running processes and their status

> Syntaxt jobs [options] jobID

#### 24. kill Command:
> The kill command is used to terminate an unresponsive process manually.
> Syntax kill [signal_option] pid
>
> Where PID is the proces ID used to reference a particular process

#### 25. ping Command:
> The ping command is used to trouble and see if a server is reachable or not
>
> Syntaxt: ping [option] [hostname_or_IP_address]


#### 26. wget Command:
> The wget command lets you download files from the internet.

> Syntax: wget [option] [url]

#### 27. uname Command:
> The uname command tells you details of your Linux system and harware
>
> Syntax: uname [option] (uname -a)


#### 28. top Command:
> The top command will display all running processes and a dynamic real-time view of the current system.
>Syntax: top


#### 29. history Command:
> The history command will list upto 500 commands you have executed.
> Syntax: history
>


#### 30. man Command:
> The man command provides a user manual of any command or utility you run in the terminal.
> Syntax: man [command name]


#### 31. echo Command:
> The echo command display line of text or string using the standard output.
> Syntax: echo [option] [string]

#### 32. zip and unzip Commands:
> The zip command is used to compress files into a ZIP file/directory.
> Syntax: zip [option] zipfile file1 file2
>
> Example -> You have a file named note.txt and you want to compress into archive.zip in the same directory,

```
   zip archive.zip note.txt
```

For the unzip command, we use this to un archive files

> Syntax: unzip [option] filename.zip


#### 33. hostname Command:
> The hostname command is used to know the system's hostname.
> Syntax: hostname [option]



#### 34. useradd, userdel Commands:
> Since Linux is a multi-user operating system, more than one user can use the system at the sametime.
> Command useradd is used to create a new user account while the 
> Syntax: useradd [option] username

> To set the password, we use the

> passwd password_combination

> Usecase:

> useradd dev

> passwd 12345
>

#### 35. apt-get Command:
> The apt-get (Advanced Package Tool) helps you retrieve information and bundle fro authenticated sources to manage, update, remove and install softwares packages and their dependencies.

>Syntax: apt-get [options] (command)


#### 36. nano, vi, jed Command:
> The nano and vi commands comes pre-installed with the operating system. They are used to edit and manage files via text editors. jed does not come pre-installed with Linux (Ubuntu)

> Syntax: nano filename

> Syntax: vi filename


#### 37. alias, unalias Commands:
> The alias command allows you to create shortcut with the same functionality as a command, filename or text

> Syntax: alias Name=String

> alias k='kill'

on the other hand unalias deletes the alias
> Syntax: unalias [alias_name]


#### 38. su Command:
> The su command allows you to run commands as a different user with administrative previleges


>su [options] [username [argument]]


#### 39. htop Command:
> The htop command monitors system resources and server processes in real time.
 
> htop [options]

#### 40. ps Command:
> The ps command produces a snapshot of all the running processes in your system.

