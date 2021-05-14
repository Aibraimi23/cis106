##Cat command
* The cat command is used for displaying the content of a file
* Car is short for concatenate which is the commands intended use
* Concatenation means joining two strings together
##Tac command
* The Tac command is used for displaying the content of a file in reverse order in a line by line basis
* The tac command can also concatenate files in reverse order
##More
* The more command is a pager program used for displaying the content of a text file one page at a time
* Usage:
  * more + file to view
##Less
* The less command is another pager program that displays the content of a file 1 page at a time
* Less is faster than more when dealing with large files since it loads 1 page at a time
* Usage:
  * less + file to view
##Head
* The head command displays the top N number of lines of a given file. By default, it prints the first 10 lines. If more than one file name is provided then data from each file is preceded by its file name
* Usage:
  * head + option + file
##Tail
* The tail command displays the last N number of lines of a given file. By default, it prints the last 10 lines. If more than one file name is provided then data from each file is preceded by its file name
##Cut 
* The cut command is used to extract a specific section of each line of a file and display it to the screen
* Usage:
  * cut + option + file
##Paste
* The paste command is used to join files horizontally in columns 
* Usage:
  * paste + option + file
##Sort 
* The sort command is used for sorting files
* Sorting means arranging the content of the file in a particular order
* The sort command supports sorting:
  * Alphabetically
  * In reverse order
  * By number
  * By month
* Sort can be used ignoring case sensitivity 
* The sort command follows this order unless specified otherwise:
  * Lines starting with a number will appear before lines starting with a letter
  * Lines starting with a letter that appears earlier in the alphabet will appear before lines starting a letter that appears later in the alphabet
  * Lines starting with a lowercase letter will appear before lines starting with the same letter in uppercase
  ##Wc
  * The wc command is used for printing the number of line, characters, and bytes in a file
  * Usage:
    * wc + option + file
  ##Tr
  * The tr command is used for translating or deleting characters from standard output
  * Usage:
    * Standard output | tr + option + set + set
  ##Diff
* The diff command compares files and display the differences between them
* Usage:
  * diff + option + file1 + file2
##Grep
* The grep command is used to match a string pattern from a file or standard output when using the pipe
* Usage:
  * grep + option + pattern to match + file
  * Standard output + pipe (|) + grep + pattern + pattern to match
##Rev
* The rev command is used for reversing the characters position in a given text
* Usage:
  * rev + file
##I/O Redirection

