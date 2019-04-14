0) emacs -nw myfirst.txt


Type a text:

==========
one two
three five six
one 
two four
=========



1) Move cursor to the beginning of the file and search for "one" using Ctrl+s.
   Each time a string is found, press Ctrl+s again to find the next instance.
2) Move cursor to the end of the file with Esc Shift >. Use Ctr+r to search for "two" backward.
3) Move cursor to the end of "three" on the second line, cut " five six" with Ctrl+k,
   paste it back with Ctrl+y, move cursor to the end of the second "one" and paste again with Ctrl+y
4) Save the buffer with Ctrl+x Ctrl+s
5) When you move the cursor up and down, notice the line number changing on the bottom bar
6) Do "Esc+x column-number-mode". Now if you move the cursor horizontally,
   you'll also see column number as well
7) Open another buffer, with Ctrl+x Ctrl+f, type the file name "mysecond.py"
8) Type the following:

=========
#!/usr/bin/env python
print("hello")
========
Notice that emacs recognized that this is python
(on the bottom bar it says that it is in Python mode).
It would highlight and format the code accordingly.

9) Check out what buffer names you have with Ctrl+x Ctrl+b. A window would open listing
   the buffers. Close the window with Ctrl+x 1.
10) Open the first buffer: Ctrl+x b, then type the buffer/file name: myfirst.txt
11) Move the cursor to the middle of the file, insert a line,
    put a cursor on the empty line and do: Esc+x insert-file, Enter,
    type mysecond.py and the second file will be inserted
    into the first file
12) Open the second window below: Ctrl+x 2
13) Go to the other window with Ctrl+x o
14) It shows the same file. Instead switch there to the other buffer mysecond.txt
15) Return to "myfirst.txt" buffer with Ctrl+x o
16) Close the other windows with Ctrl+x 1
17) Use Ctrl+x Ctrl+s to save all the buffers to files, Ctrl+x Ctrl+w saves only the current buffer
18) Try using Ctrl+e and Ctrl+a to move to the end and the beginning of some line
19) Exit the file with Ctrl+x Ctrl+c. If you have some unsaved buffers, you'll be prompted to save them.
20) Open myfirst.txt in emacs again
21) Replace all "one" with "hundred" by typing Exc+x replace-string, Enter, one, Enter, hundred, Enter
22) Notice "Tab" works for command completion in the bar like in shell
23) Exit emacs


