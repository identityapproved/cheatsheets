---
Tags: #terminal/tools/zsh 
Medium: #zsh-vi-mode
---
Tags: #terminal/tools/zsh 
Medium: #zsh-vi-mode
Created: 10.02.2023 19:10
Links: 
	 [git:zsh-vi-mode](https://github.com/jeffreytse/zsh-vi-mode) 
___

Use `ESC` or `CTRL-[` to enter `Normal mode`.

### History

-   `ctrl-p` : Previous command in history
-   `ctrl-n` : Next command in history
-   `/` : Search backward in history
-   `n` : Repeat the last `/`

### Movement

-   `$` : To the end of the line
-   `^` : To the first non-blank character of the line
-   `0` : To the first character of the line
-   `w` : [count] words forward
-   `W` : [count] WORDS forward
-   `e` : Forward to the end of word [count] inclusive
-   `E` : Forward to the end of WORD [count] inclusive
-   `b` : [count] words backward
-   `B` : [count] WORDS backward
-   `t{char}` : Till before [count]'th occurrence of {char} to the right
-   `T{char}` : Till before [count]'th occurrence of {char} to the left
-   `f{char}` : To [count]'th occurrence of {char} to the right
-   `F{char}` : To [count]'th occurrence of {char} to the left
-   `;` : Repeat latest f, t, F or T [count] times
-   `,` : Repeat latest f, t, F or T in opposite direction

### Surround

There are 2 kinds of keybinding mode for surround operating, default is `classic` mode, you can choose the mode by setting `ZVM_VI_SURROUND_BINDKEY` option.

1.  `classic` mode (verb->s->surround)

-   `S"` : Add `"` for visual selection
-   `ys"` : Add `"` for visual selection
-   `cs"'` : Change `"` to `'`
-   `ds"` : Delete `"`

2.  `s-prefix` mode (s->verb->surround)

-   `sa"` : Add `"` for visual selection
-   `sd"` : Delete `"`
-   `sr"'` : Change `"` to `'`

#### How to select surround text object?

-   `vi"` : Select the text object inside the quotes
-   `va(` : Select the text object including the brackets

Then you can do any operation for the selection:

1.  Add surrounds for text object

-   `vi"` -> `S[` or `sa[` => `"object"` -> `"[object]"`
-   `va"` -> `S[` or `sa[` => `"object"` -> `["object"]`

2.  Delete/Yank/Change text object

-   `di(` or `vi(` -> `d`
-   `ca(` or `va(` -> `c`
-   `yi(` or `vi(` -> `y`

### Increment and Decrement

In normal mode, typing `ctrl-a` will increase to the next keyword, and typing `ctrl-x` will decrease to the next keyword. The keyword can be at the cursor, or to the right of the cursor (on the same line).