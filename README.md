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

## Getting help `C-h` and...

- `(key)` describes help for the key
- `b` list the bindings for the current buffer
- `m` describe mode

## Basics

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
Open `~/.emacs.d/init.el` to do more customizations for emacs

### Editing

`c-y` pastes

`c-k` deletes to the end of the line

`c-/` is undo

### Query replace

`M-% string RET newstring RET`

### Movement

`C-v` moves down a page

`M-v` moves up a page

`C-l` centers page on cursor

`C-a` move to beginning of line `C-e` move to end of line (just like bash)

`m-m` move to first non whitespace letter

`m-f` move forward one word `m b` move back one word

`C-s` regex search. Hit again to move through the matches `C-r` does reverse search

`M-<` moves to beginning `M->` moves to end

`M-g g` go to line

### Selection (marking regions)

`C-space` to mark and then move the point (using stuff above) to select more. You can then hit backspace to delete.

Or perhaps use `M-x replace-string` to replace text inside the region

Select all is `C-x h`

### Cut, paste, etc

`C-w` Kill region (cut) `M-w` Copy region (copy)
`C-y` yank (paste) `M-y` Cycle through kill ring after yanking
`M-d` Kill word
`C-k` Kill line

### Other editing commands

`C-j` New line and indent
``M-/` Hippy expand (auto-complete)

### Links 

- http://www.gnu.org/software/emacs/manual/html_node/emacs/index.html#Top The Emacs manual, dl PDF
- https://www.masteringemacs.org/reading-guide Apparently one of the best resources
- http://www.ic.unicamp.br/~helio/disciplinas/MC102/Emacs_Reference_Card.pdf Reference card
- http://sachachua.com/blog/wp-content/uploads/2013/05/How-to-Learn-Emacs8.png Pretty picture


### Windows

`C-x o` switch window
`C-x 1` delete all over windows (doesn't delete buffers)
`C-x 2` split window horizonatlly
`C-x 3` split window vertical
`C-x 0` delete current window`

### Git

`M-x magit-status` is synonumous with git status. Remember you can close all "windows" (different from buffers!) with q.

You can move the cursor thing to the modified files and hit `tab` to see what changes you've made. Within this you can press `s` to stage or `i` to add to `.gitignore`. `k` will discard uncommited changes to a file.

`c` opens the commit menu.

`F` opens the pull menu

`C-x v L` is history `l` is verbose history

#### Commit and push

Once you're in the commit menu do `-a` to enable "all" then type `c` again to do commit. Type your commit message and then `C-c C-c` to save it.

To just commit certain files, hit `s` on selected files. `S` will select all.

To ammend a commit use `e` instead of `c`

To push do `P-P`

### Font sizes

`C-x C-+` increase font size `C-x C- -` to decrease
