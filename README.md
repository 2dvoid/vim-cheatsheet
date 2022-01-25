# Vim Language Based Cheat Sheet
My personal cheat sheet for Vim

## Vim Language Structure:
```
Verb + Modifier + Noun
```

## Insert Mode:
```
i         # insert before the cursor (insert)
I         # insert at the beginning of the line
a         # insert after the cursor (append)
A         # insert at the end of the line
o         # open a new line below the current line (open)
O         # open a new line above the current line
C         # delete rest of the line from the cursor position and enter insert mode
s         # delete character under the cursor and enter insert mode (substitute)
S         # delete current line and enter insert mode
Esc       # exit insert mode
```

## Verb:
- **Standard Verbs:**
```
d         # delete something (delete)
y         # copy something (yank)
c         # delete something and enter insert mode (change)
v         # visually select (visual)
```
- **Single Character Verbs:**
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

## Modifier:
```
i         # inside
a         # around
NUM       # number (e.g: 1,2,3)
t         # searches for a character forward and stops before it (till)
T         # searches for a character backward and stops before it
f         # searches for a character forward and lands on it (find)
F         # searches for a character backward and lands on it
/         # search upto the next match
```

## Noun:
- **Motions:**
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
)         # move to next sentence
(         # move to previous sentence
}         # move to next paragraph
{         # move to previous paragraph
%         # move to the matching parenthesis
H         # move cursor to top of the screen (High)
M         # move cursor to middle of the screen (Middle)
L         # move cursor to bottom of the screen (Low)
gg        # move to the first line of the document
G         # move to the last line of the document
````
- **Text Objects:**
```
w         # word
s         # sentence
p         # paragraph
"         # double quoted string
'         # single quoted string
`         # back quoted string
t         # HTML tag block
) or b    # parenthesized block
} or B    # brace block
]         # bracketed block
>         # single tag

```

## Scrolling:
```
zz             # scroll the screen so the cursor is at the middle
zb             # scroll the screen so the cursor is at the bottom
zt             # scroll the screen so the cursor is at the top
Ctrl + b       # move back one full screen
Ctrl + f       # move forward one full screen
Ctrl + d       # move forward 1/2 a screen
Ctrl + u       # move back 1/2 a screen
Ctrl + e       # scroll the screen up
Ctrl + y       # scroll the screen down
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

## Tips:
- **Always try to avoid Visual Mode**
- **Difference between <code>dw</code> and <code>daw</code>:** The difference is in the allowed cursor position. For example, to delete a word using dw the cursor must be at the start of the word, any other position would delete only part of the word; however, daw allows the cursor to be at any position in the word.
