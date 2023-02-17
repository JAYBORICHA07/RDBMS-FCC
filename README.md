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

Relational Databases by Building a Mario Database
Notice that the prompt changed to let you know that you are now interacting with PostgreSQL. First thing to do is see what databases are here. Type \l into the prompt to list them.


he databases you see are there by default. You can make your own like this:
CREATE DATABASE database_name;
The capitalized words are keywords telling PostgreSQL what to do. The name of the database is the lowercase word. Note that all commands need a semi-colon at the end. Create a new database named first_database.
if you don't get a message after entering a command, it means it's incomplete and you likely forgot the semi-colon. You can just add it on the next line and press enter to finish the command.
You can connect to a database by entering \c database_name. You need to connect to add information.
You should see a message that you are connected. Notice that the prompt changed to second_database=>. So the postgres=> prompt before must have meant you were connected to that database. A database is made of tables that hold your data. Enter \d to display the tables.
Looks like there's no tables or relations yet. Similar to how you created a database, you can create a table like this:
CREATE TABLE table_name();


Note that the parenthesis are needed for this one. It will create the table in the database you are connected to. Create a table named first_table in second_database.
You can view more details about a table by adding the table name after the display command like this: \d table_name. View more details about your second_table.
Tables need columns to describe the data in them, yours doesn't have any yet. Here's an example of how to add one:
ALTER TABLE table_name ADD COLUMN column_name DATATYPE;


Add a column to second_table named first_column. Give it a data type of INT. INT stands for integer. Don't forget the semi-colon. 😄
Those are some good looking columns. You will probably need to know how to remove them. Here's an example:
ALTER TABLE table_name DROP COLUMN column_name;


Drop your age column.
A common data type is VARCHAR. It's a short string of characters. You need to give it a maximum length when using it like this: VARCHAR(30).
Add a new column to second_table, give it a name of name and a data type of VARCHAR(30)
