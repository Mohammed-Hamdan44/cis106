---
Name: Mohammed Hamdan
Class: CIS106 Fall 23
---

# Week Report 7

## Cat Command
* Cat Command is used for displaying content of a file. 
* formula: cat + option + files to display
* Examples: cat todo.lst, cat ~/Documents/todo.lst

## tac command
* tac command is used for displaying the content of a file in reverse order
* formula: tac + option _ files to display 
* tac todo.md
* tac ~/Documents/todo.md

## head command
* the head command displays the top N number of lines in a given file. 
* formula: head + options + files
* examples: head ~/Documents/book/dracula.txt, head -5 ~/Documents/book/dracula.txt

## tail command
* tail command displays the bottom N number of lines in a given file
* formula: tail + options + files
* examples: tail ~/Documents/book/dracula.txt, tail -5 ~/Documents/book/dracula.txt

## cut command
* cut command is used to extract a section and display the file to a screen
* formula: cut + options + files
* examples: cut -d ':' -f1/etc/passwd, cut -d ':' -f1,7 /etc/passwd

## paste command
* paste command is used for joining files horizontally in columns
* formula: paste + options + files
* examples: paste .users.lst ip_address.lst, paste -d ':' .users.lst

## sort command
* sort command is used for sorting files
* formula: sort + option + files
* examples: sort users.lst, sort -u users.lst

## wc command
* wc command is used for printing the number of lines, characters and bytes in a file. 
* formula: wc + options + files
* examples: wc -m users.txt, wc -l users.txt

## tr command
* tr command is used for translating or deleting characters from standard output
* formula: tr + option + set + set
* examples: cat file.txt | tr '_' ','   cat program.py | tr "[:spce:]" 't/'

## diff command
* diff command compares files and displays the differences between them
* formula: diff + option + file1 + file2
* examples: diff cars.csv cars-backup.csv, diff -y cars.csv cars-backup.csv

## sed command 
* sed command is used for processing and manipulating text
* formula: sed + option + files
* examples: sed 's/pattern/replacement/' file.txt, sed 's/pattern/replacement/g' file.txt, sed -n '/pattern/p' file.txt,sed '/pattern/d' file.txt,  sed 's/$/ additional text/' file.txt

## awk command
* awk command is a versatile to process files
* formula: awk + 'option' + text
* examples: awk '{print $1, $3}' file.txt, awk '$2 > 50 {print $1, $2}' data.txt, awk '{sum+=$2} END {print "Average:", sum/NR}' data.txt, awk '{gsub("old", "new", $0); print}' file.txt, awk '/pattern/' file.txt