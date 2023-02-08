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

## Modes:
- Normal
- Insert - typing text
- Visual - equivalent mouse operations
- Command - `:`
- Visual Line

Go out _insert mode_ -> `esc`, `C-c`, `C-[`

### In normal mode
`zz` - recenter screen
Cursor remember last furthest known location.
`x` - delete char
`w` - move through words delemeters
`b` - -//- back
`dd` - delete line (or `Vd`)
`u` - undo
`yy` - yank(copy) line
`p` - paste below
`P` - paste above moving current line down

### Visual Mode
`v` - hightlight part of the line
`V` - -//- all line

`:reg` - tracked things you delete(`d`) and yanked(`y`)
`d` -> kept in order of history all way down
`y` ->  preserved for only one `0` register

### Insert Mode
`a` - open cursor inside(right)
`i` - open cursor outside(left)
`I` - first non-whitespace char in the beginning of the line
`A` - always to full end of the line
`o` - open cursor on new line respects indenting
`O` - insert new line above shifting down others
