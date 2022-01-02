# Vim Language Based Cheat Sheet
My personal cheat sheet for Vim

## Vim Language Structure:
```
Verb + Modifier + Noun
Visual_Mode + Verb
```

## Modes:
### Insert Mode:

```
i         # insert before the cursor (insert)
I         # insert at the beginning of the line
a         # insert after the cursor (append)
A         # insert at the end of the line
o         # open a new line below the current line (open)
O         # open a new line above the current line
C         # delete rest of the line from the cursor and enter insert mode
s         # delete character under the cursor and enter insert mode (substitute)
S         # delete current line and enter insert mode
Esc       # exit insert mode
```

### Visual Mode:
```
v         # character-wise visual mode
V         # line-wise visual mode
aw        # mark a word
ab        # a block with ()
aB        # a block with {}
ib        # inner block with ()
iB        # inner block with {}
```

## Verb:
```
d         # delete something (delete)
c         # delete something and enter insert mode (change)
y         # copy something (yank)
```

## Modifier:
```
i         # inside
a         # around
NUM       # number (e.g: 1,2,3)
t         # searches for a character and stops before it (till)
f         # searches for a character and lands on it (find)
```

## Noun:
```
h         # move to one character left
j         # move to one row down
k         # move to one row up
l         # move to one character right
w         # move to the beginning of the next word
b         # move to the beginning of the previous word
W         # move to the beginning of the next word after a white space
B         # move to the beginning of the previous word before a white space
e         # move to the end of the next word
E         # move to the end of the word after whitespace
0         # move to the start of the line
$         # move to the end of the line
}         # move to next paragraph
{         # move to previous paragraph
gg        # move to the first line of the document
G         # move to the last line of the document
5G        # go to line 5
````

## Command:
```
dd        # delete a line (delete)
D         # delete to the end of the line from the cursor
yy        # copy a line (yank)
p         # paste after cursor (paste)
P         # paste before cursor
x         # delete character under cursor (delete)
X         # delete character left of cursor (backspace)
r         # replace character under cursor with another character (replace)
R         # replace character under cursor with multiple characters
J         # join line below to the current one
u         # undo
Ctrl + r  # redo
```

## Search:
```
/pattern       # search for pattern
?pattern       # search backward for pattern
n              # next search result
N              # previous search result
:noh           # remove highlighting of search matches
```

## Exit:
```
:w              # save the file, but don't exit (write)
:w !sudo tee %  # save out the current file using sudo
:wq or :x or ZZ # save and quit
:q              # quit (fails if there are unsaved changes)
:q! or ZQ       # quit and throw away unsaved changes
```
