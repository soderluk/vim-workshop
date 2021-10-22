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

## Searching text

You can search for text by entering the search key `/{word to search}<CR>`, then navigate to the next occurrence with `n` and previous occurrence with `N`. You can start searching backwards by entering `?` instead of `/`.

Search for string: `/{string}`\
Jump to character: `t`\
Jump onto character: `f`\
Search for other instances of the word under your cursor: `*`\
Go to the next instance when you've jumped to a character (with `f` or `t`): `;`\
Go to the previous instance when you've jumped to a character (with `f` or `t`): `,`


# Assignment 1

Please read the instructions in the `assignment-1.txt` file, and try out the verbs, modifiers and nouns.
In the first assignment we also learn to move around in a normal text file. Open the file in vim, and start working on it.
If you need help, just ask.

[Assignment-1](assignment-1.txt)

[Introduction](01-introduction.md) || [Next up, changing text](03-changing-text.md)
