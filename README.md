# rituraut

A SIMPLE TEXT EDITOR


->What is  a simple text-based editor ?
	 Simple Text-based Editor. It is a command-shell based text editor
that enable user to edit, save, and view any type of file in ASCII format. The original
purpose of this program is to demonstrate pointers, memory allocations/de-allocations,
file input or output, and string search techniques in C.


->Features that a simple text editor should consists of :
1>Edit the current line
2>Move one line up
3>Move one line down
4>Delete the current line
5>Display the contents of the buffer
6>Add a line after the line at which you are navigating
7>Save changes and exit to main menu
8>Exit discarding any changes
9>Show the list of commands


->The Structure of the Program
	A huge buffer is used to read from and store all the text. The buffer is written in a linked-
list structure, the text file is break down and represented in list of nodes. A second buffer
is also used for tracking purposes for the undo feature in this illustration. Adding,
replacing, deleting a line or a block involves simple iteration processes that involve O(n)
complexity. Saving, reading, quitting, and undo are also bounded in the same complexity.


->How to use the program?
	After compilation, an executable would be automatically generated (default executable
file name for C Programming Language is a.exe). Run the program with desired text file
name in shell command line. Usage, “./try <filename>” .


->Limitations of the program would be:
	The text program only reads in ASCII format text files. Any other file would not be able to work properly with the editor.


->Other aspect of the program
	Undo is a complex operation that involves many different programming techniques in
this demonstration. The operation would require a history of the command and the
information the user had type. Using this information, the software tracks the amount of
code that it needs to bring back or erase.
One other aspect of the program is to free the allocated memory when it is no longer to be used. In Java, this is automatically done with the Java’s Garbage Collector. However, in C we will need to use Malloc () to reserve a memory space for our linked-list and use Free() when discarding the unused memories.