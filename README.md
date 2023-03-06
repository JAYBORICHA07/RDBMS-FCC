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

# Relational Databases by Building a Mario Database

- Notice that the prompt changed to let you know that you are now interacting with PostgreSQL. First thing to do is see what databases are here. Type \l into the prompt to list them.

### ``` CREATE DATABASE databasename;```
- This command is used to create the database;

### ```CREATE TABLE tablename(column_name type constrains,...);```
- This command is used to create the tables in database.

### ```INSERT INTO table_name(col1,col2,..) values(val1,val2,...);```
- This command is used to add the data into different columns. we can also add mutiple data like this ```INSERT INTO table_name(col1,col2,..) values(val1a,val1b,...),(val1b,vaal2b);```
### ```ALTER TABLE tablename task WHERE condition;```
- Alter table is used to alter the table
- in task we can do various tasks like drop column, add column, add constrains, remove constrains, rename columns,rename table, rename database and many more.
- in the condition the place where we want to alter or change the table is to be written.

## here is some example of alter commmand

- Add a new column to a table: ``` ALTER TABLE table_name ADD COLUMN new_column_name TYPE;```

- Drop a column in a table : ``` ALTER TABLE table_name DROP COLUMN column_name;```

- Rename a column: ```ALTER TABLE table_name RENAME column_name TO new_column_name;```

- Add a primary key to a table.: ``` ALTER TABLE table_name ADD PRIMARY KEY (column,...);```

- Remove the primary key from a table : ``` ALTER TABLE table_name DROP CONSTRAINT primary_key_constraint_name;```

- Rename a table : ``` ALTER TABLE table_name RENAME TO new_table_name;```

### DETETE COMMANDS
- This is how we can delete a row :  ```DELETE FROM table_name WHERE condition; ```

- Delete all rows of a table: : ```DELETE FROM table_name;```

- Delete specific rows based on a condition: ```DELETE FROM table_name WHERE condition;```

### SELECT COMMAND 
- select command is used to select or view perticular info from table

## HERE ARE SOME EXAMPLE OF SELECT COMMAND

- select all data from a table: ``` SELECT * FROM table_name;````

- select data from specified columns of all rows in a table: ``` SELECT column_list FROM table;```

-  select data from a table with a filter: ``` SELECT * FROM table WHERE condition;```

- select joint data : ```SELECT *  FROM table1 FULL OUTER JOIN table2 ON conditions;```