# Text objects

So, you're working on text in vim, be it README's, code or a novel, it doesn't matter, you'll be working with text objects in any case.
You should start learning to use the text objects to your advantage, e.g. instead of moving to the beginning of a sentence and deleting it, you can do that from within the text you're manipulating.

## Word text objects

Inside word: `iw`\
Around word: `aw`

So, what you can do to delete around a word, `daw`. Consider the following: "Delete around word." if you run `daw` on the word `around`, you'll get `Delete word.`. If in turn you run `diw` you'll get `Delete  word.`, notice the extra space there. Any other actions can be run against these, e.g. change, delete, etc.

## Sentence text objects

Inside sentence: `is`\
Around sentence: `as`

The same applies for sentences as for words. You can e.g. change a sentence from wherever you are within the sentence. Let's consider the sentence: `This sentence I want to keep. This sentence is not too good, and I want to change it to something else. This again I want to keep.` Running `cis` on the word `good,` vim will delete everything from the start of the sentence and put you in insert mode at the beginning of your new line.

Let's try it out:

`This sentence I want to keep. This sentence is not too good, and I want to change it to something else. This again I want to keep.`

There are other text object types that work in a similar fasion, and that includes:

Paragraphs: `ip` and `ap`\
Single quotes: `i'` and `a'`\
Double quotes: `i"` and `a"`\
Parenthesis, brackets, braces, back ticks: `i(` and `a(`, `i[` and `a[`, `i{` and `a{`, also `i<backtick>` and `a<backtick>`.\
Tags: `it` and `at` (Think about HTML tags)

These might come in handy when you're editing HTML or any other code, since you can easily change something that's inside quotes, delete or replace. 

# Assignment 2

Please read the instructions in the `assignment-2.txt` file, and try working on undoing, redoing and working on text objects. In the second assignment we're going to use the things we have learnt this far.

[Assignment 2](assignment-2.txt)

[Introduction](01-introduction.md) || [Next up - Visual mode](05-visual-mode.md)
