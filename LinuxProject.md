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

cp sqlite_commands.sh /home/ubuntu/unixcommands

cp filename1.txt filename2.txt filename3.txt /home/username/Documents


