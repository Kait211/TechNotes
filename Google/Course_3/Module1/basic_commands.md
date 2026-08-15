# Windows
- GUI (Graphical User Interface)
- CLI (Command Line Interpreter)

# Linux
- Command line

The command line interpreter in Linux us called a shell, and the language that we'll use to interact with this shell is called Bash

# Basic Operating System Navigation 
- Navigating from one directory to another
- Getting file information
- Removing files and directories 

# File and Text Manipulation
- Searching through your directories
- Find a specific file
- Copying and Pasting 
- Chaining commands 

In Windows, file systems are assigned to drive letters which look like C, D, or X

### Root directory
The parent for all other directories in the file system

The root directory of C: would be written C:\, and the root directory of X: would be written X:\

Subdirectories are separated by backslashes (\), unlike Linux, which uses forward slashes (/).

The C: drive root folder is what we call a parent directory and the contents inside are considered child directories 

Similar to Windows commands and parameters, a flag is a way to specify additional options for a command 

The -a or all flag shows all files including hidden ones 

### Absolute path
One that starts from the main directory 

### Relative path
The path from your current directory 

- pwd shows you what directory you are currently in

- if your press D then tab other directories starting with D will come up

- typing history in command line will show all commands that you used 

- can use ctrl r to search thru commands

In Windows, the hotkey for copy is Ctrl-C, and the hotkey for paste is Ctrl-V

- copy in Linux is cp

### Wildcard
A character that's used to help select files based on a certain pattern 

- if I do cp *.jpg then directory I want to save them to i can copy all jpegs in one directory to another 

- can save a file with spaces in the name by creating name like this. mkdir 'My new folder'

### -Recurse
List the contents of the directory

### -Verbose
Copy doesn't output anything to the CLI by default unless there are errors 

# example of cp on powershell
PS C:\Users\Owner\Desktop> cp Picture.webp C:\Users\Owner\Documents

- mv allows us to rename files for instance mv .\blue_doc.txt yellow_doc.txt, I can also use it to move documents to other directories in a similar way That I show how to copy a file to another directory 

- To remove a directory, recursively remove the files with -r. Also, folders with spaces in the name have to be escaped with \.