# LinuxPracticeProjects
A Repository for my LinuxProject
## sudo command
This is the short command for superuserdo. It allows one perform task that require administrative or root permission
- Syntax:
sudo (command e.g apt upgrade)
- sudo apt upgrade
![sudo](./img/1.sudo.png)

## pwd
This command  means present working directory. This command return the full current path. it accepts 2 options -L or -logical prints environment variable contend, including symbolic links.
-P or -physical prints the actual path of the current directory

- Syntax: pwd [option]
![pwd](./img/2.pwd.png)

## cd
This allows the user navigate through the Linux files and directories. Your current working directory requires the full path or the directory name. The cd command without and option takes you to the home page, however only users with sudo privileges can execute it

- Syntax: cd CommandsLinux

![cd](./img/3.cd.png)

- Some shortcuts
cd ~[username]goes to another user's home directory
cd.. move one directory up
cd- moves to the previous directory

## ls
This command list files and directories within the system. Running it without a flag returns the  current working directory content
- Syntax ls [option]
- ls /home/ubuntu

![ls](./img/3.ls.png)
- other options include
ls -R, ls -a, ls -lh 
![ls](./img/4.lsb.png)

## cat
This command stands for Concatenate, it is one of the most frequently used linux commands. Its function is to list, combine and write file content to standard output

- Syntax: cat [option]
![cat](./img/5.cate.png)
To Merge files and store the output in another file
- cat file1 file2 > file3
![MergeFile](./img/5.cateb.png)
To displays content in reverse order
- tac filename.txt 

![ReverseOrder](./img/5.catec.png)


## cp
This command is used to cope files or directories and their content

To cope one file from the current directory to another directory.
- cp devopsFile /home/ubuntu/WorkSpace
 ![copyToDirectory](./img/6.cp.png)
 To copy the content of a new file in the same directory to a new directory
 - cp devopsFile devopsFile2
 ![CopyFilesToNewDirectory](./img/6.cpb.png)
 To  copy an entire dirctory, pass the -R flag before typing the source directory, followed by the destination directory
 - cp -R /home/ubuntu/WorkSpace /home/ubuntu/WorkSpace_backup
 ![CopyAllDirectory](./img/6.cpc.png)

 ## mv
 mv command is used to move and rename files and directories. It dosen't produce an output upon execution

To move a file to a new directory
- mv devops1 /home/ubuntu/WorkSapce_backup

 ![move](./img/7.mva.png)

 To rename a file
 - mv devops2 devops2_remane
 ![rename](./img/8.mvrename.png)

 ## mkdir command
 This command is used to create one or multiple directosries at once and set permission for them. 
 - syntax :mkdir [option] directory_name
 ![mkdir](./img/8.mkdir.png)
  
  To make a directory inside Music Folder
  - mkdir Music/Songs
  ![mkdirFolderInsideFolder](./img/8.mkdirSong.png)

  To create a directory between two existing folders we use the -p or -parents. 
  
 -  For example mkdir -p Music/2020/Songs

  To  create directory with full read, write and execute permissions for all users we use
  
   - mkdir -m777 directory_name

  To Prints a message for each created directory 

  - mkdir -v directory_name

  ## Rmdir command
This command is used to permanently delete an empty directory

![removedir](./img/8.mvrename.png)

## rm Command
The rm command is used to delete files within a directory
 - syntax: rm filename
 ![DeleteFile](./img/9.rm.png)

 To delete multiple file
 - syntax: rm filename1 filename2 filename3
 ![RemoveMultiple](./img/10.rmMultiple.png)
 
 Some acceptable options include:

 -i prompts system confirmation before deleting a file

 -f allows the system to remove without a confirmation

 -r deletes files and files and directories recursively

 
 ## touch command
 This command allows a user create an empty file
 - syntax: touch filename
 ![touch](./img/11.touch.png)

 ## locate command
 This command is used to create a find a file in the database
 - syntax: locate -i school*note

 ![locate](./img/12.locate.png)

 ## find command
 This command is used to search for files within a specific directory and perform subsequent operations

 -syntax:       find [option] [path] [expression]

 ![find](./img/13.find.png)

 Other options include:

 find -name filename.txt: This is used to find files in the current directory
 
 find ./ -type -name diretoryname : This is used to look for directories

 ## grep command
This command is used to look for a word by searching through all the text in a specific file.

- syntax: grep values sql_commands.sh

![grep](./img/14.grep.png)

## df command
This command is used to report the system disk space usage, shown in percentate and kilobyte(KB)
- syntax: df [options] [file]
- options include -m displays information on the file system usage in MBs. df-k displays file system usage in KB. DF -T shows all the file system type in a new column

To see the current directory system disk space usage in a human-readable format
- df -h
![df](./img/15.df.png)
## du command
This command is used to check how much space a file of a directory takes up. Note that the directory path must be specified 

- syntax :du [option]filepath

Some of the options include: -s which offers the total size of a specified folder, -m provides folder and file information in MB, -K displays information in KB, -h informs the last modification date of the displayed folders and files
-
![du](./img/16.du.png)

## head
This command is used to view the first ten lines of a text in a file. To change the number of files shown we include an option

- syntax:head [option] [file]

![head](./img/17.head.png)
The image shows the option -n in use
![head](./img/17.heada.png)

## tail
This command displays the last ten lines of a file. It allows the user to check if a file has new records or if there is an error message

- syntax : tail [option] [file]
![tail](./img/18.tail.png)

## diff 
This command compares the two contents of a file line by line, after the analyzes it displays the one that do not match. This command is used by programmers to alter a program instead of rewriting the entire sourc code

- syntax: diff [option] file1 file 2
Some of the accepted options include -c which displays the difference between two files in a context form, -u displays the output without redundant infromation, -i makes the diff command case insensitive
![difference](./img/19.difference.png)














