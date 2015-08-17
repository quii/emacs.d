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
Open `~/.emacs.d/init.el` to do more customizations for emacs

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

### Selection (marking regions)

`c-space` to mark and then move the point (using stuff above) to select more. You can then hit backspace to delete.

Or perhaps use `m-x replace-string` to replace text inside the region

### Cut, paste, etc

`c-w` Kill region (cut) `m-w` Copy region (copy)
`c-y` yank (paste) `m-y` Cycle through kill ring after yanking
`m-d` Kill word
`c-k` Kill line

### Other editing commands

`c-j` New line and indent
``m-/` Hippy expand (auto-complete)

### Links 

- http://www.gnu.org/software/emacs/manual/html_node/emacs/index.html#Top The Emacs manual, dl PDF
- https://www.masteringemacs.org/reading-guide Apparently one of the best resources
- http://www.ic.unicamp.br/~helio/disciplinas/MC102/Emacs_Reference_Card.pdf Reference card
- http://sachachua.com/blog/wp-content/uploads/2013/05/How-to-Learn-Emacs8.png Pretty picture


### Windows

`c-x o` switch window
`c-x 1` delete all over windows (doesn't delete buffers)
`c-x 2` split window horizonatlly
`c-x 3` split window vertical
`c-x 0` delete current window`

### Git

`m-x magit-status` is synonumous with git status. Remember you can close all "windows" (different from buffers!) with q.

You can move the cursor thing to the modified files and hit `tab` to see what changes you've made

`c` opens the commit menu.

### Commit and push

Once you're in the commit menu do `-a` to enable "all" then type `c` again to do commit. Type your commit message and then `C-c C-c` to save it.

To just commit certain files, hit `s` on selected files. `S` will select all.

To ammend a commit use `e` instead of `c`

To push do `P-P`

