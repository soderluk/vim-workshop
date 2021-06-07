# Changing text

## Modes in vim

Vim has a bunch of different modes that you need to understand before we move on.

`Normal mode`: This is the mode where you start when you open a file in vim, remember this, as you can't just open a file and start typing to enter text. Normal mode is also known as `Command mode` as this is where you also can type your commands, e.g. `dd` to delete text.\
`Insert mode`: Insert mode is where you make changes to your file.\
`Visual mode`: Visual mode is a way to select text, so that you can perform different operations on the highlighted text, such as copy it, surround it with quotes, brackets or similar.\
`Ex mode`: This is the command prompt mode, which you enter with the colon (:), this will drop you to a command line at the bottom of the vim window. Note that you need to be in normal mode to drop to command mode.

## Basic options for changing and inserting

Insert before the cursor: `i`\
Append after the cursor: `a`\
Insert at the beginning of the line: `I` (that's a capital i)\
Append at the end of the line: `A`\
Open a new line below the current: `o`\
Open a new line above the current: `O`\
Replace the one character under your cursor: `r`\
Replace the character under your cursor but keep typing afterwards: `R` (more or less constant replace mode)\
Change whatever _movement_, e.g. a word (w), sentence (s) or paragraph (}): `c<m>` (where m is the movement e.g. `cw`)\
Change the current line from where you're at: `C`\
Change up to the question mark: `ct?`\
Substitute from where you are to the next command (noun): `s`\
Substitute the entire current line: `S`
Change the case of the character under your cursor: `~` (the tilde sign, works also on visual mode selected text)

## Basic options for deleting text

Delete the character under the cursor: `x`\
Delete the character before the cursor: `X`\
Delete whatever _movement_: `d<m>` (e.g. `dw` to delete a word.)\
Delete the current line: `dd`\
Delete from where you are to the next period: `dt.`\
Delete to the end of the line: `D`\
Join the current line with the next line: `J` (delete whatever is between the lines)

## Undoing and redoing

Undo: `u`\
Redo: `Ctrl-r`\
Undo all latest changes on current line: `U`

## Repeating actions

You can use the dot `.` to repeat the last action you did. Let's say you delete a word with `dw`, now you can run `5.` which deletes 5 more words.
Now combining this with a search and some editing, it's quite powerful:
Search for a text, e.g. `/Delete` and then hit enter. You will find all the instances of the word `Delete`. Now press `A` to append to the end of the line some text (full command): `/Delete<Enter>A" hello"<ESC>` (search for the word Delete, append " hello" at the end of the line). Now that we have the action, we can repeat that on all the instances by running `n.` which means, search for the next instance (`n`) and repeat the last action, e.g. Appending the text " hello". 

## Copying, cutting and pasting text

Yank selection: `y`\
Yank the current line: `yy`\
Cutting text: `dd` (delete current line into a buffer, can be pasted, also when deleting a single character it's in the buffer ready for pasting)\
Paste the copied text after the current cursor position: `p`\
Paste the copied text before the current cursor position: `P`


[Introduction](introduction.md) || [Next up - Text objects](text-objects.md)
