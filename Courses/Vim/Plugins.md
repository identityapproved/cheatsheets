---
Tags: #course/vim
Medium: #course #vim 
---
Tags: #course/vim
Medium: #course #vim 
Created: 09.02.2023 10:17
___

## [vim-plugins](https://github.com/junegunn/vim-plug):
- [fzf-vim](https://github.com/junegunn/fzf.vim) (not [[Terminal#^38ef5c]])
	- GFiles - Git files 
	- Files `[PATH]`
	- Create `nnoremaps` for `:cnext`/`:cprev`
	- `:Rg` - ripgrep
	- `:Lines` - search thro the buffers
	- `:History:` - search in command history
	- 
- [vim-smoothie](https://github.com/psliwka/vim-smoothie) - This (neo)vim plugin makes scrolling nice and _smooth_. (every time you press `Ctrl-D` or `Ctrl-F`)
- [vim-airline](https://github.com/vim-airline/vim-airline)
- [vim-bufferline](https://github.com/bling/vim-bufferline)
- [vim-css-color](https://github.com/ap/vim-css-color)
- [vim-devicons](https://github.com/ryanoasis/vim-devicons)
- [typescript-vim](https://github.com/leafgarland/typescript-vim)
- [vim-jsx-pretty](https://github.com/MaxMEllon/vim-jsx-pretty)
- [vim-javascript](https://github.com/pangloss/vim-javascript)
- [vim-graphql](https://github.com/jparise/vim-graphql)
- [vim-sayonara](https://github.com/mhinz/vim-sayonara)
- [NERDTree](https://github.com/preservim/nerdtree)
- [coc-nvim](https://github.com/neoclide/coc.nvim)
- [indentline](https://github.com/Yggdroot/indentLine)


### QuickFix:
- `:grep` + what you are looking for + file or ext `**/*.ext`
- `:copen` - open qflist
- `:h cdo` - execute command in all buffers and `:wa` - write all
#### `:h getqflist()`:
- `:echo getqflist()`
- ordering with __neovim__ + __lua__(`:luafile %`):
```lua
vim.fn.setqflist(vim.fn.sort(vim.fn.getqflist(), function(a, b)
	local a_text = a.text
	local b_text = b.text
	local a_num = a_text:sub(9, #a_text - 2)
	local b_num = b_text:sub(9, #b_text - 2)
	if tonumber(a_num) > tonumber(b_num) then
		return 1
	end
	return -1
end))
```

### Search and replace:
- `/` + searching thing or can use regex (but dont use regex)
- `n` or `N` - navigating
- `:set hls ic` - highlight search result, ignorecase / `:nohls`
- replace:
	- highlight text + `/s/foo/bar
	- `%s/foo/bar/gc` -> `g` - global, `c` - ask (y/n)

### Macro Mode:
- `q` - start/stop recording
- `C-a` - increment first number in the line
- `@_` - repeat recorded

### Registers:
- is a _key_ -> _value_ 
- `"qy` - yank to _q key_
- `"wp` - paste from _w key_