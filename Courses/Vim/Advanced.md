---
Status: #status/inprogress
Tags: #course/vim
Medium: #course #vim 
---
Status: #status/inprogress
Tags: #course/vim
Medium: #course #vim 
Created: 09.02.2023 10:17
Links: 
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