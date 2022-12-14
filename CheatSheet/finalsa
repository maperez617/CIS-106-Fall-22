---
Name: Marcelo Perez
Course: CIS 106
Semester: Fall 22
---
# Final Exam Study Assignment 
## Question 1

**awk** is a scripting language use for processing and displaying text. Awk can work with a text file or from standard output
**Usage** awk + options + {awk command} + file + file to save (optional)
**Examples**
Print first and last field of /etc/passwd file
awk -F: '{print $1," = ",$NF}' /etc/passwd
Print the first and 3 field with line numbers
awk -F: '{print NR,$1,$3}' /etc/passwd
Convert the first field to upper/lower case
awk -F: 'print toupper($1)}' /etc/passwd

**cat** is used for displaying the content of a file. 
**Usage** cat + option + files(s) to display
**Examples**
Display content of a file using absolute path
cat ~/Documents/todo.lst
Display content of a file with line numbers
cat -n ~/Documents/todo.lst
Display content of a file with line numbers excluding empty lines
cat -b ~/Documents/todo.lst

**cp** is a command that copies directories from a source to a destination.
**Usage** cp + files to copy + destination 
**Examples** 
To copy a file 
cp Downloads/wallpapers.zip Picture/
to copy a directory with absolute path
cp -r ~/Downloads/wallpapers ~/Pictures/
To copy multiple files in a single command 
sudo cp -r script.sh program.py home.html assets/ /var/www/html

**cut** is used to extract a specific section of each line of a file and display it to the screen.
**Usage** cut + option + file(s)
**Examples**
Display a list of all the users in the system with their login shell
cut -d ':' -f1,7 /etc/passwd
Cut a file excluding a given field
cut -d ',' --complement -s -sf3 users.txt
Display a list of all the users in your system 
cut -d ':' -f1 /etc/passwd

**grep** is used to search text in a given file. Grep works on a line by line basis.
**Usage** grep + option + search criteria + file(s)
**Example**
Search any line that contains the word 'dracula' regardless of the case in the given file:
grep -i 'dracula' ~/Documents/dracula.txt 
Search for all the lines that do not contain the word 'war'
grep -v 'war' ~/Documents/Books/war-and-peace.txt
Search for all the lines that ends with the string "nologin"

**head** is used to display the top N number of lines of a given file. By default, it prints the first 10 lines. 
**Usage** head + option + file(s)
**Examples** 
Display the first 10 lines of a file 
head ~/Documents/Book/dracula.txt 
Display the first 5 lines of a file
head -5 ~/Documents/Book/dracula.txt
Display the first 20 lines of a file
head -20 ~/Documents/Book/dracula.txt

**ls** is used for displaying all the files inside a given directory. 
**Usage** ls + option + directory to list
List all the files in a given directory by file size 
ls -S ~/Documents
List all the files in a given directory by extension 
ls -X ~/Documents
List all the files in a given directory in reverse order 
ls -r ~/Documents

**man** are documentation files that describe Linux shell commands, executable programs, system calls, special files, and so forth. 
**Usage** man + option
**Examples** 
View the entire manual 
man ls
Open the man page of the passwd command 
man passwd
Show all the available pages of a command
man -a passwd

**mkdir** is used for creating a single directory or multiple directories 
**Usage** mkdir + the name of the directory 
**Examples** 
Create a directory using absolute path 
mkdir ~/wallpapers/forest
Create multiple directories 
mkdir wallpapers/cars wallpapers/cities wallpapers/forest
Create a directory with a parent directory at the same time
mkdir -p wallpapers_others/movies

**mv** moves and renames directories
**Usage** mv + source + destination 
**Examples** 
move a file from a directory using relative path
mv Downloads/homework.pdf Documents/
move a file using absolute path
mv ~/Downloads/theme /usr/share/themes
move multiple directories 
mv games/ wallpapers/ rockmusic/ /media/student/flashdrive/ 

**tac** is used for displaying the content of a file in reverse order. 
**usage** tac + option + file(s) to display
**Examples**
Display the content of a file using absolute path
tac ~/Documents/todo.md
Display the content of a file located in pwd
tac todo.md

**tail** is used to display the last N number of lines of a given file. By default it prints the last 10 lines. 
**Usage** tail + option + file
**Examples** 
Display te last 10 lines of a file
tail ~/Documents/Book.dracula.txt 
Display the last 5 lines of a file
tail -5 ~/Documents/Book.dracula.txt

**touch** is used for creating files
**Usage** touch + destination + file name
**Examples**
To create multiple files in pwd
touch list.txt script.py names.csv
To create a file using absolute path
touch ~/Downloads/games.txt 
To create a file with a space in its name
touch "list of foods.txt"

**tr** is used for translating or deleting characters from standard output
**Usage** standard output | tr + option + set + set
**Examples**
translate one character to another like a period to a comma
cat file.txt | tr '.' ','
translate white space into tabs
cat program.py | tr "[:space:] '\t'
translate tabs into space 
cat file.py | tr -s "[:space:]" ' '

**tree** lists the files in the cwd showing a diagram
**Usage** tree + location 
**Examples**
Show a tree of your class directory 
tree ~/Documents/CIS106
Show a tree of your home directory 
tree ~/ 
Show a tree of the games folder
tree ~/Downloads/Games

**vim** is a line text edior is included all POSIX compliant operating systems
**Usage** vim

## Question 2
How do you work with multiple terminals open? 
right click inside the terminal and click on new window

How to work with manual pages?
type man in the terminal and a specific command like man pwd to quit the manual press q

How to parse (search) for specific words in the manual page?
man ls | grep 'group' while open the manual for the ls command and search for lines with the word group

How to redirect output (> and |)?
The > command allows you to direct the output of a command to a file and the |(pipe) allows you to redirect the standard output of a command to the standard input of another.

How to append the output of a command to a file?
**Examples**
Save the output of a command to a file.
ls -lA ~ > all-files-inhome.txt
Save the error generated by a command to a file 
ls -lA downloads/ 2> error-of-ls
Save the error and success to the same file
ls -lA downloads/ Pictures &> alloutput.txt

How to use wildcards? 
**Wildcards** 
1. (*) The star matches anything and nothing and matches any number of characters. Example: mv *.py ~/Documents/Pythonfiles
2. (?) The question mark matches precisely one character Example ls f??e.*
3. ([]) the brackets wildcard match a single character in range Example ls f[aeiou]*

How to use brace expansion? 
Brace expansion {} is not a vildcard but another feature of bash that allows you to generate arbitrary strings to use with commands
**Examples** 
To create a whole directory structure in a single command
mkdir -p music/{jazz,rock}/{mp3files,videos,oggfiles}/new{1,2,3}
