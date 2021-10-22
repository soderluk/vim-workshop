# Bonus stuff

Here's a few bonus things that will help you on your journey to the vim world.

## Macros

Macros are awesome! You can record macros into different registers, and there's a LOT of registers that you can use.

Start recording a macro into the `a` register: `qa`\
Stop recording the macro: `q`\
Play the macro: `@a`

The macro will be stored in the register that comes after the verb `q` so you have all the alphabetical letters to your disposal, so `qz` stores the macro in the `z` register. Then to replay the macro, just type `@z`.

## Registers

Registers are even more awesome! They're not only used for storing macros, but a lot more.

Use `:reg` to see the registers that are available, you'll see a list of registers starting with a double quote `"<register>`. 
The unnamed register `""` will contain any text that you delete with `d`, `c`, `x`, `s` or yank with `y`. This means that you really can't lose your text ever. Let's say you by accident delete a whole line, and then do something stupid, so you can't use undo anymore to get the text back. You can use the registers to recover the deleted text from the numbered registers which are automatically populated by vim. This means that the text you just yanked will be populated in the "0 register. To paste it you can use `"0p` in normal mode.

Vim also have 4 read only registers: `".`, `"%`, `":` and `"#` these contain useful information

Last inserted text: `".`\
Current file path: `"%`\
Last executed command: `":`\
Alternate file name: `"#` (last edited file)

There are also a few special registers in vim, such as the expression register and search register.

The expression register `"=` can be used to run different expressions. In insert mode, you can type `Ctrl-r =` to enter an expression, let's say `2+2<CR>` which will write `4` in the text. You can also run system commands such as `Ctrl-r =` then `system('ls')<CR>` which will paste the output of the `ls` command in your buffer.

The search register contains the latest text that you searched for. Simple and effective. 

You can also use `Ctrl-r <register>` when in the command mode, e.g. if you're running a substitution `:%s/foo/bar/g` you can insert any register at any point by just pressing e.g. `Ctrl-r /` to insert the text from the last search.

We also have the clipboard register available to us, this is found in `"+` (the plus register). So to copy a text to the clipboard in vim, visually select the text you want to copy, then type `"+y` and you have the text in your clipboard. 

## The vim help

The vim help is a lifesaver. It has answers to everything you need to know. Just type `:help` or `:h` to open the help.
If you have a specific thing you need to find, use `:h <the thing>` e.g. `:h gq` to see the formatter information.
Any key combination can also be searched for in different modes, e.g. `:h CTRL-R` to see the help on redoing stuff. If you recall, there's also `Ctrl-r` in insert mode, so lets get the help for that, `:h i_CTRL-R` and thus you get help on the key combination in insert mode.

## Where to go from here?

So, now we've just only skimmed the surface of editing and moving around in vim. We didn't really even skim the surface, as we started out with the very very basics. From here you should start looking into your `vimrc` file which will configure vim to your liking. Start out minimalistic, only include things that you really need, and learn to use those tools well first. After that you can continue setting up different plugins and so on.

If you want, we could have another workshop that handles some plugins and configuring vim to your liking.

# Assignment 3

Please read the instructions in the `assignment-3.txt` file, and make the necessary changes to the file.

[Assignment 3](assignment-3.txt)

# Sources and tutorials

[Vim registers: The basics and beyond - By Brian Storti](https://www.brianstorti.com/vim-registers/)\
[Learn Vim For the Last Time: A Tutorial and Primer - By Daniel Miessler](https://danielmiessler.com/study/vim/)\
[Openvim](https://www.openvim.com/)


[Introduction](01-introduction.md)
