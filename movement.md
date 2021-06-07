# Moving around in vim

Forget about arrows (except in `insert` mode), since we have the home-row (the row where `hjkl` are located).

The following movements operate one line/one character at a time:

Move down: `j`\
Move up: `k`\
Move left: `h`\
Move right: `l`

## Moving around the current line:

Move to the beginning of the line: `0` (that's a zero)\
Move to the end of the line: `$`\
Move to the first non-blank character in the line: `^` (I can't seem to get this to work, probably better on US keyboard layout)\
Jump to right before the next quotes: `t"`\
Jump and land on the next quotes: `f"`

## Moving around words:

Move forward one word: `w`\
Move backward one word: `b`\
Move to the end of the word: `e`

## Moving by sentence or paragraph:

Move forward one sentence: `)`\
Move backward one sentence: `(`\
Move forward one paragraph: `}`\
Move backward one paragraph: `{`

## Moving within the screen

Move to the top of the screen: `H`\
Move to the middle of the screen: `M`\
Move to the bottom of the screen: `L`\
Move to the top of the file: `gg`\
Move to the bottom of the file: `G`\
Move up half a screen: `^U`\
Move down half a screen: `^D`\
Page down: `^F`\
Page up: `^B`

_Note: the hat ^ means that you should press Ctrl+<character>, e.g. Ctrl+F for Page down_

Bonus:

Jump to your previous navigation location: `Ctrl-i`\
Jump back to where you were: `Ctrl-o`

# Assignment 1

Please read the instructions in the `assignment-1.txt` file, and try out the verbs, modifiers and nouns.
In the first assignment we also learn to move around in a normal text file. Open the file in vim, and start working on it.
If you need help, just ask.

[Assignment-1](assignment-1.txt)

[Introduction](introduction.md) || [Next up, changing text](changing-text.md)
