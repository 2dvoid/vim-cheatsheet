# Vim Cheat Sheet
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
### Standard Verbs: (takes noun as arguments)
```
d         # delete something (delete)
c         # delete something and enter insert mode (change)
y         # copy something (yank)
```
### Single Character Verb: (takes no argument)
```
x         # delete character under cursor (delete)
X         # delete character left of cursor (backspace)
r         # replace character under cursor with another character (replace)
R         # replace character under cursor with multiple characters
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
```
