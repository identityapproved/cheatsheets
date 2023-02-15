---
Tags: #course/vim
Medium: #course #vim 
---
Tags: #course/vim
Medium: #course #vim 
Created: 09.02.2023 10:17
___

### Horisontal and Vertical Movement

- `c` - works like `d`, but after deleting -> incert mode
- `D` = `d$`
- `C` = `c$`
- `s` =  works like `x`, but after deleting -> incert mode
- `f` - find the char and jump on it -> `;` - next / `,` - prev
- `t` = `f` but jump to the char, not on it.
- `T` & `F` - reverse
- `{` & `}` - jumps to next/prev paragraf (blanc lines)
- `C-d` `C-u` - half page jumping
- `[m` / `]m` and `[M` / `]M` - jumps on curly braces
- `%` - pair jumper (`[](){}""`)
- `di{` - delete inside braces 
- `ci{` - + incert after
- `vi{` - hl insides
- `da{` - delete with curly brackets (same with `va{` & `ca{`)
- in visual mode `o` jump between selections
- `diw` - delete word inside (`ciw` & `viw`)
- `viW` - hl word inside whitespaces (`diW` & `ciW`)
- `dap` - delete all paragraf
- `gv` - hl previous hl

```vimrc
vnoremap <leader>p "_dP # paste withou loosing original one
vnoremap <leader>y "+y # yanked to the system clipboard
nnoremap <leader>y "+y # in normal mode
nnoremap <leader>Y gg"+yG # yank all file to sys clip

vnoremap J :m '>+1<CR>gv=gv
vnoremap K :m '>-2<CR>gv=gv
```

### Buffers
- `C-o` - backward
- `C-i` - forward
- `:bn` / `:bp` - next/previous
- `:bd` - unload buffer and delete from buffer list
- `:bw` - really delete the buffer

### Indentation 
```
>>   Indent line by shiftwidth spaces
<<   De-indent line by shiftwidth spaces
5>>  Indent 5 lines
5==  Re-indent 5 lines

>%   Increase indent of a braced or bracketed block (place cursor on brace first)
=%   Reindent a braced or bracketed block (cursor on brace)
<%   Decrease indent of a braced or bracketed block (cursor on brace)
]p   Paste text, aligning indentation with surroundings

=i{  Re-indent the 'inner block', i.e. the contents of the block
=a{  Re-indent 'a block', i.e. block and containing braces
=2a{ Re-indent '2 blocks', i.e. this block and containing block

>i{  Increase inner block indent
<i{  Decrease inner block indent
```