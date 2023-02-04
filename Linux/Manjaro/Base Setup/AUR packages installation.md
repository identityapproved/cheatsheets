For manual installation, download the PKGBUILD file from this repository. 
Run:
```shell
makepkg -cf
```
which will create a .pkg.tar.zst file. 
Then:
```shell
sudo pacman -U <filename.pkg.tar.zst>
```

Or you can use an AUR Helper such as yay and run
```shell
yay -S git-clone-url # from https://aur.archlinux.org/packages
```
