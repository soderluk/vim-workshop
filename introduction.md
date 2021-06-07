# Vim basics workshop

## What is vim?

Vim is the one editor you'll ever need. It's a text editor that usually comes with every single Linux distro as default. If not `vim̀` then it's usually `vi`. OK, this is something that all `vim` enthusiasts say, but I'm not THAT enthusiastic about it. Maybe I'll be there some day, though, since I only lately started using it actively. 

Vim is many times the editor that people start using, but ends up abandoning because there's a LOT of things to learn when starting out.

The most used meme about vim is, "How to quit vim?"... It seems to be something that people has difficulties figuring out.

Hint: use `:q` to quit :)

## The vim motions

We have verbs, e.g. actions we take and which can be performed on nouns:

Delete: `d`\
Change: `c`\
Yank: `y`\
Visually select: `v` (`V` for whole line)

We have modifiers that are used to describe what we want to do to the nouns:

Inside: `i`\
Around: `a`\
Number: `<NUM>`\
Searches for something and stops before it: `t`\
Searches for something and lands on it: `f`\
Find a string: `/`

We have the nouns that are something you do _to_:

Word: `w`\
Sentence: `s` or `)`\
Paragraph: `p` or `}`\
Tag: `t`\
Block: `b`

So how do we use these building blocks then? It's easy, just combine them together `verb + modifier + noun`, e.g:

Delete two words: `d2w`\
Yank inside paragraph: `yip`

Note that you can use the same set up for movement as well, e.g. move 3 words forward: `3w`

## Working with your files

Open your _file_ in vim: `vim file`
Write your changes to the file: `:w`
Quit without saving: `:q!`
Write your changes and exit vim: `:wq`
Save your file as: `:saveas /path/where/to`
Faster way to do `:wq`: `ZZ`

[Next up, moving around](movement.md)
