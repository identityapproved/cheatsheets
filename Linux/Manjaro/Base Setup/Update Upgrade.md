Update distro:
```shell
sudo pacman -Syu
```
-   `-S`: synchronize your system’s packages with those in the official repo
-   `-y`: download fresh package databases from the server
-   `-u`: upgrade all installed packages

or:
```shell
sudo pacman -Syyu
```
Extra y forces the package manager to download/update the packages database for all repositories regardless of whether there is any change in the versions. Use if the normal upgrade command is producing an error or failing to retrieve the latest software releases.
