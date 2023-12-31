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


#### 16. du Command:
> We can use the df command to check how much space a file or directory takes up

> Syntax: du [file_name]/[directory_name]

#### `Output`

<img width="521" alt="Screenshot 2023-08-25 at 08 03 53" src="https://github.com/tundek/DevOps_Projects/assets/15998669/6d99c4f7-b0b1-4a18-b37c-c67709d84b6e">


#### 17. head Command:
> The head command is used to display the first 10 lines of a text file/document
> Syntax: head [file_name]

<img width="651" alt="Screenshot 2023-09-01 at 18 15 16" src="https://github.com/tundek/DevOps_Projects/assets/15998669/91a760f5-1ed0-4dae-8ca7-c7ba6bd49784">



#### 18. tail Command:
> The tail command is used to display the last 10 lines of a text file/document
> Syntax: tail [file_name]

<img width="676" alt="Screenshot 2023-09-01 at 18 15 33" src="https://github.com/tundek/DevOps_Projects/assets/15998669/c2a3b97c-a342-4ca2-8c0a-81d1010b9541">



#### 19. diff Command:
> The diff command (different) is used to compare the contents of two files and displays the part that do not match.
> Syntax: diff [option] [file_name1] [file_name2]

#### `Output`

<img width="819" alt="Screenshot 2023-08-25 at 08 17 49" src="https://github.com/tundek/DevOps_Projects/assets/15998669/76dba3c0-2a8a-4e3e-9b08-26089012619a">

#### 20. tar Command:
> The tar command archives multiple files into TAR file.
> Syntax: tar [options] [archive_file] [file or directory to be achived]

#### `Output`
<img width="794" alt="Screenshot 2023-09-01 at 21 12 21" src="https://github.com/tundek/DevOps_Projects/assets/15998669/0026a975-401d-46ce-b132-78b7a94952b7">


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

#### `Output`
<img width="798" alt="Screenshot 2023-09-01 at 21 27 42" src="https://github.com/tundek/DevOps_Projects/assets/15998669/2f02b69d-b14f-4351-afb8-ac0708cc3bd5">
<img width="823" alt="Screenshot 2023-09-01 at 21 27 26" src="https://github.com/tundek/DevOps_Projects/assets/15998669/678ed36d-af63-49c2-b339-3d56048550b3">



#### 23. Jobs Command:
> A job is process started by the shell. The job command will display all the running processes and their status

> Syntaxt jobs [options] jobID
<img width="769" alt="Screenshot 2023-09-01 at 21 45 37" src="https://github.com/tundek/DevOps_Projects/assets/15998669/ea554ede-f90a-4278-8df8-555c083c792d">



#### 24. kill Command:
> The kill command is used to terminate an unresponsive process manually.
> Syntax kill [signal_option] pid
>
> Where PID is the proces ID used to reference a particular process
<img width="642" alt="Screenshot 2023-09-01 at 21 43 56" src="https://github.com/tundek/DevOps_Projects/assets/15998669/533ab271-0ff2-42c0-9a48-4be7c195a250">


#### 25. ping Command:
> The ping command is used to troubleshoot and see if a server is reachable or not
>
> Syntaxt: ping [option] [hostname_or_IP_address]

<img width="851" alt="Screenshot 2023-09-01 at 21 29 53" src="https://github.com/tundek/DevOps_Projects/assets/15998669/ec3c543a-801a-445b-aec8-fc21105c5aa0">



#### 26. wget Command:
> The wget command lets you download files from the internet.

> Syntax: wget [option] [url]
>
<img width="1406" alt="Screenshot 2023-09-01 at 21 48 23" src="https://github.com/tundek/DevOps_Projects/assets/15998669/6d98c789-a069-4fd0-83f8-58591f160f37">


#### 27. uname Command:
> The uname command tells you details of your Linux system and harware
>
> Syntax: uname [option] (uname -a)
<img width="557" alt="Screenshot 2023-09-01 at 21 49 51" src="https://github.com/tundek/DevOps_Projects/assets/15998669/6eca695a-a8e7-4f13-9b5b-3712f41fbaf7">


#### 28. top Command:
> The top command will display all running processes and a dynamic real-time view of the current system.
>Syntax: top
<img width="1407" alt="Screenshot 2023-09-01 at 21 48 57" src="https://github.com/tundek/DevOps_Projects/assets/15998669/f22f6fdd-fc00-4664-a336-30522570b7cd">



#### 29. history Command:
> The history command will list upto 500 commands you have executed.
> Syntax: history
<img width="1025" alt="Screenshot 2023-09-01 at 21 50 48" src="https://github.com/tundek/DevOps_Projects/assets/15998669/4aca3418-fb7b-4dcc-a550-1e6e6f7f0738">




#### 30. man Command:
> The man command provides a user manual of any command or utility you run in the terminal.
> Syntax: man [command name]
Example: man ls
<img width="1417" alt="Screenshot 2023-09-01 at 21 51 40" src="https://github.com/tundek/DevOps_Projects/assets/15998669/7392c276-0a76-4ae2-9f73-c068758c4416">



#### 31. echo Command:
> The echo command display line of text or string using the standard output.
> Syntax: echo [option] [string]
<img width="802" alt="Screenshot 2023-09-01 at 21 53 55" src="https://github.com/tundek/DevOps_Projects/assets/15998669/ed32cada-bdcf-43d8-bee7-26281b4faadc">


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
<img width="941" alt="Screenshot 2023-09-01 at 21 57 09" src="https://github.com/tundek/DevOps_Projects/assets/15998669/52298007-c04c-4f25-98a7-ba3955d42de1">




#### 33. hostname Command:
> The hostname command is used to know the system's hostname.
> Syntax: hostname [option]
<img width="616" alt="Screenshot 2023-09-01 at 21 57 41" src="https://github.com/tundek/DevOps_Projects/assets/15998669/a8597e19-8e55-4d6f-bee9-76afe9d64907">



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
<img width="895" alt="Screenshot 2023-09-01 at 22 38 30" src="https://github.com/tundek/DevOps_Projects/assets/15998669/109c95fa-d2e8-41f6-b114-f2a585a92222">



#### 35. apt-get Command:
> The apt-get (Advanced Package Tool) helps you retrieve information and bundle fro authenticated sources to manage, update, remove and install softwares packages and their dependencies.

>Syntax: apt-get [options] (command)
<img width="1270" alt="Screenshot 2023-09-01 at 22 40 53" src="https://github.com/tundek/DevOps_Projects/assets/15998669/943582b6-9984-4f25-8c0f-a0fa2a4bad5d">
<img width="1419" alt="Screenshot 2023-09-01 at 22 40 45" src="https://github.com/tundek/DevOps_Projects/assets/15998669/89f0b8fd-dd61-4966-8126-d0c81a8d0ac9">
<img width="986" alt="Screenshot 2023-09-01 at 22 40 00" src="https://github.com/tundek/DevOps_Projects/assets/15998669/b39cdeec-f216-4e53-84f8-68bf55996516">




#### 36. nano, vi, jed Command:
> The nano and vi commands comes pre-installed with the operating system. They are used to edit and manage files via text editors. jed does not come pre-installed with Linux (Ubuntu)

> Syntax: nano filename

> Syntax: vim filename
<img width="695" alt="Screenshot 2023-09-01 at 22 52 01" src="https://github.com/tundek/DevOps_Projects/assets/15998669/86bfac5b-b782-4765-a861-94fbc880ca14">
<img width="1402" alt="Screenshot 2023-09-01 at 22 50 51" src="https://github.com/tundek/DevOps_Projects/assets/15998669/308ec6cf-88fc-454d-9dee-e6e34799227d">




#### 37. alias, unalias Commands:
> The alias command allows you to create shortcut with the same functionality as a command, filename or text

> Syntax: alias Name=String

> alias k='kill'

on the other hand unalias deletes the alias
> Syntax: unalias [alias_name]
<img width="605" alt="Screenshot 2023-09-01 at 22 57 16" src="https://github.com/tundek/DevOps_Projects/assets/15998669/2c801872-ea1b-4cf5-b878-5abcfe9ebee2">
<img width="731" alt="Screenshot 2023-09-01 at 22 54 58" src="https://github.com/tundek/DevOps_Projects/assets/15998669/65defccd-1336-4b03-b826-52ce3c3813e7">



#### 38. su Command:
> The su command allows you to run commands as a different user with administrative privileges
>su [options] [username [argument]]
<img width="733" alt="Screenshot 2023-09-01 at 23 00 17" src="https://github.com/tundek/DevOps_Projects/assets/15998669/51c36bf1-6ae7-4af3-b746-fe64876c0531">


#### 39. htop Command:
> The htop command monitors system resources and server processes in real time.
 
> htop [options]
<img width="973" alt="Screenshot 2023-09-01 at 23 04 53" src="https://github.com/tundek/DevOps_Projects/assets/15998669/a5606206-8b54-4ffe-a116-502a34c859da">



#### 40. ps Command:
> The ps command produces a snapshot of all the running processes in your system.
> htop [options]
> 
 <img width="459" alt="Screenshot 2023-09-01 at 23 05 29" src="https://github.com/tundek/DevOps_Projects/assets/15998669/51a617a3-c6dd-4a16-84f6-9b28b692fe53">

> 

