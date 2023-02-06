## TWM 
- a window manager that automatically tiles the windows into mutually, non-overlapping frames. This is a different then traditional floating/stacking window managers.
- list-based/tree-based & dynamic/manual

### Common layouts:
- master and stack
- grid
- monocle/full/max
- spiral/fibonacci
- dwindle
- floating

REFERENCED: 
► [dwm.suckless](https://dwm.suckless.org/) 
► [xmonad](https://xmonad.org/) 
► [qtile](http://www.qtile.org/) 
► [awesomewm](https://awesomewm.org/) 
► [i3wm](https://i3wm.org/) 
► [herbstluftwm](https://herbstluftwm.org/) 
► [bspwm](https://github.com/baskerville/bspwm)

Cons:
- take too much time and effort to configure
- GUI apps look like crap in twm
- keyboard-centric paradigm conflicts with apps that use mouse
- re-arranging, moving and resizing windows is a chore
- some UI elements are not displayed correctly and require manual configuration
- no Alt-Tab or App Overview functionality
- most relevant apps already include tiling functionality one way or another

KDE Plasma solution -> KWin Scripts:
- Krohnkite (DWM)
(To enable configuration, you must perform the following in command-line:
```
mkdir -p ~/.local/share/kservices5/
ln -s ~/.local/share/kwin/scripts/krohnkite/metadata.desktop ~/.local/share/kservices5/krohnkite.desktop
```
A configuration button will appear in `KWin Scripts` in `System Settings`.)

## Krohnkite Default Key Bindings

^3c216d

| Key | Action |   
| ----------- | ----------- |   
| Meta + J | Focus Down/Next |   
| Meta + K | Focus Up/Previous |
| Meta + H | Left |
| Meta + L | Right |
| Meta + Shift + J | Move Down/Next |
| Meta + Shift + K | Move Up/Previous |
| Meta + Shift + H | Move Left |
| Meta + Shift + L | Move Right |
| Meta + I | Increase |
| Meta + D | Decrease |
| Meta + F | Toggle Floating |
| Meta + `\` | Cycle Layout |
| Meta + Return | Set as Master |
| Meta + T | Use Tile Layout |
| Meta + M | Use Monocle Layout |
| _unbound_ | Use Spread Layout |
| _unbound_ | Use Stair Layout |
