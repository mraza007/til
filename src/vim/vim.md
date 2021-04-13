## Vim Notes
These are learning notes when learning `vim key bindings`

## Vim has three modes

- `INSERT` : You can use `i` for the insert mode
- `VISUAL` : You can use `v` for visual mode.
- `NORMAL MODE` : just press `ESC` to get into normal mode

## Basic Navigation

- In order to get into insert mode use `i`.
- `gg` takes you to the first line of the document.
- `Shift-G` takes you to the last line of the document.
- You can also move to the specfic line by `<line number> G`.
- you can use `x` to delete a character.
- you can use `u` to undo a change.
- you can also specific the number of characters you want to delete `<num of char> x`
- to delete a whole word use `dw`.
- to delete a line use `dd`.
- to number of lines use `<num of lines> dd`.
- to move one word at a time `w`.it goes to the beginning character of the word.
- to move using last character use `e`.
- to move number of words use `<num of words> w` for example `10 w` this moves 10 words.
- to move backward a word you can use `b`.
- to move number of words backward use `<num of words> b` `10 b`.
- use `0` to go to the beginning of the line.
- you use `p` to put a line to desired line number for example you can `dd` a line then `10 G` and then do `p` to put the line on line 10 
- You can replace a word or a character by using `r`.
- `Change` to get into change command you can change words by using `ce` to  get the end of the word.
- `c$` to change the entire line
- navigating using command `f`:(forward <to_word>) and uppercase does this in reverse. for example,`fe` will take to the character **e** and `Fe` will take you backward.

## Different Insert Modes.

- `A` takes to the end of the line and enters in to insert mode.
- `a` takes you into insert mode.
- `S` deletes the entire line and enters you into the insert mode.
- `s` delete the character and enters you into the insert mode.
- `o` enters you into the insert mode in the next line.
- `O` enters you into the insert mode in the preceding line.
- `C` deletes the character and enters you into the insert mode basically `$c`
- `d$` deletes everything from the cursor to the end of the line. You can use `D` to do the same thing.

## Yanking

Its the copy command in the vim editor

- to copy a word just use `yw` you can paste by using `p`.
- `yy` to copy the entire line.
- `y$` to copy from the cursor to the end of the line.

## Searching through the code/doc

- `/` search forward in the doc. then hit `n` to goto the next instance.
- `?` searches backward in the doc.

## Replacing

- You can `:%s/oldstring/newstring/g` to replace a word
- you can also give line numbers `1,2s/old/new/g`
- `:%s/old/new/gc` gives a prompt.

## Executing a command in vim
- `! <cmd>` to execute a command
- `cntrl-d` to see what commands are available
