---
Name: Mohammed Hamdan
Class: CIS 106 Fall 23
---

# Final Assignment

## Question 1 Commands
For every command in this list, include the following:
* Description
* formula/syntax
* 3 examples that you understand well

Commands:

* awk
  Description: awk is a scripting language used for processing and displaying text.
  formula/syntax: awk + options + {awk command} + file + file to save (optional)
  examples:
  awk '{print $1}' ~/Documents/Csv/cars.csv
  awk -F: '{print $1}' etc/passwd
  awk -F: '{print $NF}' etc/passwd
* cat
  Description: The cat command is used for displaying the content of a file. 
  formula/syntax: cat + option + file(s) to display
  examples:
  cat todo.lst
  cat ~/Documents/todo.lst
 cat -n ~/Documents/todo.md
* cp
  Description: copies files/directories from a source to a destination.
  formula/syntax cp + files to copy + destination
  examples:
  cp Downloads/wallpapers.zip Pictures/
  cp -r ~Downloads/wallpapers ~/Pictures/
  cp Downloads/wallpapers/* ~/Pcitures/
* cut
  Description: used to extract a specific section of each line of a file and display it to the screen.
  formula/syntax: cut + option + file(s)
  examples:
  cut -d':' -f1,3 /etc/group
  cut -d',' -f3 filename.csv
  cut -d':' -f2 /etc/passwd
* grep
  Description: grep is used to search text in a given file.
  formula/syntax: grep + option + search criteria + file(s)
  examples:
  grep 'dracula' ~/Documents/dracula.txt
  grep -i 'dracula' ~/Documents/Books/dracula.txt
  grep -in 'dracula' ~/Documents/Books/dracula.txt
* head
  Description: displays the top N number of lines of a given file.
  formula syntax: head + options + file(s) 
  examples: 
  head ~/Documents/Book/Dracula.txt
  head -5 ~/Documents/Book/Dracula.txt
  head filename.txt
* ls 
 Description: used for displaying all the files in an active directory. When no director is specified, ls displays the files in the current working directory.
 formula/syntax ls + option + directory to list
 examples: 
 ls -a
 ls -a ~/Pictures
 ls -1R ~/Pictures
* man
  Description: manual for a comman inside a linux shell.
  formula/syntax: man + command
  examples: 
  man passwd
  man ls
  man 5 passwd
* mkdir
  Description: is used for creating a directory or multiple directories.
  formula/syntax: mkdir + name of the directory
  examples: 
  mkdir wallpapers
  mkdir wallpapers/ocean 
  mkdir ~/Wallpapers/forest
* mv
  Descrtiption: moves and renames directories
  formula/syntax: mv + source + destination
  examples:
  mv Downloads/homework.pdf Documents/
  mv Downloads/english_homework.docx /media/student/flashdrive/
  mv games/ wallpapers/ rockmusic/ /media/student/flashdrive/
* tac
  Description: used for displaying the content of a file in reverse order.
  formula/syntax: tac + option + file(s) to display
  examples:
  tac todo.md
  tac ~/Documents/todo.md
  tac filename.txt
* tail
  Description: displays the last n Number of lines in a file.
  formula/syntax: tail + option + file
  examples:
  tail ~/Documents/Book/Dracula.txt
  tail -5 ~/Documents/Book/Dracula.txt
  tail filename.txt
* touch 
 Description: is used for creating files.
 formula/syntax : touch + file to create
 examples: 
  touch list
  touch ~/Downloads/game.txt
  touch "list of foods.txt"
* tr
  Description: used for translating or deleting characters from standard output
  formula/syntax: Standard output | tr + option + set + set
  examples:
  cat file.txt | tr '_', '.'
  cat program.py | tr "[:space:]" '\t'
  cat program.py | tr -s "[:space:]" ' '
* tree
  Description: displays the structure of a directory or folder in a tree-like format. It provides a visual representation of the hierarchy of directories and subdirectories, along with the files contained within them.
  formula/syntax: tree + options + file(s)
  examples
   tree /path/to/directory
   tree -L 2 /path/to/directory
   tree -a /path/to/directory

  ## Question 2

### How to work with multiple terminals open?
 - By right-click on the desktop or a file manager window and choose "Open Terminal" to open a terminal in the current directory. 
 - In one terminal you can keep using the commands and the other terminal you can use the ls command to help ensure a user is on the right track with the proper directory.
### How to work with manual pages?
 - first input man ls
 - then use spacebar to navigate to other pages
 - hit / to search then type search term and press Enter
 - press 'q' to exit manual page.
### How to parse (search) for specific words in the manual page?
 - press / to search desired term
 - then press enter to find term
### How to redirect output (> and |)?
 - Use the > operator to redirect  the output of a command to a file.  Example: ls > file_list.txt
 - Use the | operator to  send the output of one command as input to another command. Example: ls | grep "txt"
 - Then by combining both > and | together to redirect the output of a command and then pipe it to another command. -   - Example: ls -l > file_details.txt
### How to append the output of a command to a file?
 - To append the output of a command to a file, you can use the >> operator. This operator appends the output to the specified file. Example: command >> output.txt. 
### How to use wildcards (For copying and moving multiple files at the same time)?
 - Use cp command
 - Use curly brackets {}, or regular brackets ()
 - in brackets input file(s)
 - Seperate wildcard input inside a brack with commas, and can also have multiple brackets.(this should move multiple files). 
 - Example: cp {*.doc,*.pdf} ~
### How to use brace expansion (For creating entire directory structures in a single command)?
 - use mkdir command
 - then press / for the name of the directory you wanna create
 - then use curly brackets {} seperated with commas and input files you wanna create. (you can use multiple curly brackets seperated with commas and and the /)
 - Example: mkdir -p School/{F1,F2,F3}/{temp1,temp2}



  
