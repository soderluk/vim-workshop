# Visual mode

Entering the visual mode can be done simply by hitting the key `v` in normal mode.

Character based visual selection: `v`\
Line based visual selection: `V`\
Paragraph based visual selection: `Ctrl-v`

You can visually select text within any of enclosing characters such as (, [. {, dots and commas.
Use `vi(` to select text within a parenthesis (such as this). If you have nested levels, you may add a number after the verb, e.g. `v2i{`.
In the following case: `{level 1 {level 2 {level 3}}}` it of course depends on in which level you are, but if running `v2i{` inside level 3, it will select both texts within level 2 and level 3 braces. This might come in handy when programming (in a language where braces are needed...)

The most important part here is to understand that when you're in visual mode, every action you run, will be modifying the highlighted text. As an example, you can expand the selection by using `w` or `)`.

So you can select text, you can copy or cut the selected text with `y` or `d`, you can for example copy an entire paragraph and paste it below with `vipyjjp`. This command can be broken down into the following:

`v` - visually select characterwise\ 
`ip` - inside paragraph\
`y` - yank the selected text\
`jj` - move down two lines\
`p` - paste the text

Simple and elegant. Just remember what the different verbs, modifiers and nouns are. The above command is just a sequence of multiple verb+modifier+noun sets.

[Introduction](01-introduction.md) || [Next up - Macros and registers](06-macros-and-registers.md)
