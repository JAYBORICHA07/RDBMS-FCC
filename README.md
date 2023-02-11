# RDBMS-FCC
- This folder contains the RDBMS part of fcc



# Bash script
### echo :
- Echo is used to print anything in th terminal.
- i.e. [echo hello world] this command will print hello world in the terminal.

### pwd : 
   - stands for "print working directory".
   - pwd is used to know the exact location where you are, like if you are in a certain folder and you don't know the path of that folder then this command can be used to know the exact path and location of the file/folder.

### ls :  
   - ls stands for "list".
   - ls is used to know what files are in the certain folder. This command will list out all the file in the folder you are in.

### cd :
   - The cd command, also known as chdir (change directory), is a command-line shell command used to change the current working directory.

### cd .. :
   - By this command we can go one level back from the working directory.

### cd ../.. :
   - By this command we can go two level back from the working directory.

### more <filename> :
  - more is used to view (but not modify) the contents of a text file one screen at a time.

### clear :
- clear command is used to clear the terminal.

- you can add a flag to a command to use it different ways like this: ls <flag> . 
### mkdir :
- mkdir command is used to creat folder in the current working directory.

### touch :
- touch command is used to create specefic file in the current working directory.
- i.e. touch index.html will create a file named index.html in current working directory.

### flags (la —a) :
- Flags modify the operation of a command and are sometimes called options. ls is the command name, and -a -F are the flags. There are some circumstances when a parameter actually begins with a dash ( - ). In this case, use the delimiter dash dash ( — ) before the parameter.

### cp :
- cp command is used to create a copy of the contents of the file or directory specified by the SourceFile or SourceDirectory parameters into the file or directory specified by the TargetFile or TargetDirectory parameters.
- i.e. cp Src_file1 Src_file2 Src_file3 Dest_directory

### rm :
- rm command is used to remove files you no longer need. The rm command removes the entries for a specified file, group of files, or certain select files from a list within a directory.

### mv :
- You can rename them with mv like this: mv <filename> <new_filename> . mv stands for "move", it can rename or move something. Rename roboto.font to roboto.woff

### find :
- find command can be used to find files and directories and perform subsequent operations on them.
- find flags (find -name <filename>)

### rmdir :
-  rmdir is used to delete the diroctory.
- rm -r <folder> is used to delete the empty folder.

### Echo text >> File Name :
- this technique is used to insert text to certain file.

### cp -r website-boilerplate toms-website :
- with this example we can copy toms-website folder in the website-boilerplate directory.