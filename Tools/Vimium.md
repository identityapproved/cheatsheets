---
Tags: #browser/extension
Medium: #browser #vimium
---

Tags: #browser/extension #browser/extension/shortcuts
Medium: #browser #vimium
Created: 07.02.2023 15:13
Links: [vimiun github](https://github.com/philc/vimium)
___

```ad-attention
Always check language.
```

Once you have Vimium installed, you can see this list of key bindings at any time by typing `?`.

Additional advanced browsing commands:

```
]], [[  Follow the link labeled 'next' or '>' ('previous' or '<')
          - helpful for browsing paginated sites
<a-f>   open multiple links in a new tab
gi      focus the first (or n-th) text input box on the page. Use <tab> to cycle through options.
gu      go up one level in the URL hierarchy
gU      go up to root of the URL hierarchy
ge      edit the current URL
gE      edit the current URL and open in a new tab
zH      scroll all the way left
zL      scroll all the way right
v       enter visual mode; use p/P to paste-and-go, use y to yank
V       enter visual line mode
```

Vimium supports command repetition so, for example, hitting `5t` will open 5 tabs in rapid succession. `<Esc>` (or `<c-[>`) will clear any partial commands in the queue and will also exit insert and find modes.

There are some advanced commands which aren't documented here; refer to the help dialog (type `?`) for a full list.