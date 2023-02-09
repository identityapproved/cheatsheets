---
Status: #status/inprogress
Tags: #course/vim
Medium: #course #vim 
---
Status: #status/inprogress
Tags: #course/vim
Medium: #course #vim 
Links:
___

### `:set`:
- scrolloff=8
- number
- relativenumber (or rnu)

`7dd` - repeat 7 times
`d6j` - delete 6 down
`V6j` - highlight 6 lines down -> `d`
`df` -> delete from to -> `+a` <- `a` char included 
`D` - delete all the rest of the line
`dt;` - delete __till__ ;

### ~/.vimrc
- `:scriptnames` list all the .vim files that Vim loaded for you, including your `.vimrc` file.
- To create your vimrc, start up Vim and do one of the following:
```vim
:e $HOME/.vimrc
```

- location of your .vimrc file:
```vim
:echo($MYVIMRC)
```
will open it:
```
:e $MYVIMRC
```
- `:echo stdpath("config")` - where init.vim

### PopUp:
- `tab` - open popup menu, and `C-n`(next)/`C-p`(previous) to navigate
- `C-d` - open list of available

### Files and Navigation
- NetRW - default plugin
- `:Ex` / `:Vex`(vertical split) / `:Sex`(horisontal split) or `C-w + s/v`
- `C-w` - window mode for navigating through splitted w.
- `C-w + o` - close all opened splits, but not current buffer
- in `:reg` :
	- `%` is current file
	- `#` location of current file (not previous file) 
 - `C-^` - NetRW (not jump to previous file)
 - `:jumps` (`C-o` and `C-i`) - navigating through jump list
 - `Shift+%` - jumping on brackets
 - `_` - first non-space char of the line
 - `f+_` - hop to `_` 

### New Keybinding
let mapleader = " "
nnoremap <leader>pv :Vex<CR>
n -> mode "v, i, c, t"
nnore -> no recursive execution
map 
<leader>pv -> key `space`+ p + v
:Vex<CR> -> `CR` - cariage return 

### Marks:
- `m` -> mark -> + name ('A')
- ` ' ` + name of the mark moved you there
- Capital letters for Global marks / Lower for buffer scope
- can be used for main functions or classes
