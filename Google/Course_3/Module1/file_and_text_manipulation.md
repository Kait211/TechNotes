### cat, more, and less are commands that
shows contents of a file 

### Enter key
Advances the file by one line

### Space key
Advances the file by one page

the q key allows you to quit out of more and go back to the shell

- cat fruits.txt -head 10 will show the first ten lines of the file fruits and -tail 10 shows the last ten lines

### G
This moves to the end of a text file

### /word_search
This allows you to search for a word or phrase 

### nano text.txt
allows you to make changes to a text file in Linux Ubuntu

### start notepad++ text.txt
allows you to make changes to a text file in windows power shellS

Get-Help is used for PowerShell commands like Get-Help ls, and /? is used for other commands like dir such as dir /?

- can search for a word using Ctrl -f

from Notepad++, press CTRL+SHIFT+F to open the Find in Files dialog

the -Filter parameter will filter the results for file names that match a pattern 

### ls 'C:\Program Files\' -Recurse -Filter *.exe 
for instance will find all exe files under the Program Files directory 

The asterisk means match anything, abd tge .exe is the file extension for executable files in Windows 

- grep is used to find words in text

# Windows operating systems have
- stdin
- stdout
- stderr

### Pipe (|): Sends the output of one command into another command.
Example: ls | grep ".txt"
- ls → lists files
- | → passes the output to the next command
- grep ".txt" → shows only files containing .txt

### Regular expressions
Used to help you do advanced pattern-based selection


if you want to delete an non empty directory
rm -r non_empty_dir