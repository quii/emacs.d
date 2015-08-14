# my emacs config and notes

Based on https://github.com/flyingmachine/emacs-for-clojure

## stuff i like so far

- Navigating files and buffers is a breeze
- Installing packages is as pleasant as sublime text
- Tab auto-completion like bash is nice

## wut?

I learn by writing things down.

## Commands as I learn them..

Notation for emacs commands is C for Ctrl and M is for Alt

`C-x C-s` saves the file (with this config you can also just do command+s like normal)

`C-z` quits

`C-g` Stops a command if you mess up

### Buffers

`C-x b` allows you to nav open buffers or create a new one if you specify an unknown name

`C-x k` will "kill" (delete) the buffer

`C-x C-f` will open a file, use tab to make this less painful

### Commandy-stuff

Keyboard shortcuts like the ones above are just mapped to commands. You can invoke a command just by doing `M+x` and typing the name. Just like sublime's lovely thing.

### Modes

Mode is a bunch of keybindings and functions to be more productive when editing different kinds of files. Modes are either major or minor. Major would be something language specific like clojure and are usually set when you open a file (but you can use M+x to set the mode manually).

Minor modes are useful for multiple file types. 

### Package manager, whooo! 

`M-x package-list-packages` Mark packages to install with `i` and then install with `x`. 

### Editing

`c-y` pastes

`c-k` deletes to the end of the line

`c-/` is undo

### Movement

`c-a` move to beginning of line `c-e` move to end of line (just like bash)

`m-m` move to first non whitespace letter

`m-f` move forward one word `m b` move back one word

`c-s` regex search. Hit again to move through the matches `c-r` does reverse search

`m-<` moves to beginning `m->` moves to end

`m-g g` go to line


