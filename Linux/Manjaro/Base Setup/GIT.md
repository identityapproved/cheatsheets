---
Tags: #terminal/tools #terminal/tools/git #terminal/tools/ssh #linux/terminal 
Medium: #terminal #linux #git #ssh
---
Tags: #terminal/tools #terminal/tools/git #terminal/tools/ssh #linux/terminal 
Medium: #terminal #linux #git #ssh
Links:
___
Git configuration:
```shell
git config --global user.name "your_name"
git config --global user.email "your_email@example.com"
```
to summarise:
```shell
git config -l  # List Git configuration settings (same as --list)
git config -e  # Opens Git configuration in the default editor (same as --edit)
```

Creating an SSH Key Pair for User Authentication:
```shell
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
- `rsa` - an old algorithm based on the difficulty of factoring large numbers. A key size of at least 2048 bits is recommended for RSA; 4096 bits is better.
- `-t` - selected algotrithm
- `-b` - key size
- `-C` - comment appended to the end of the public key file
```Shell
cat ~/.ssh/id_rsa.pub # copy and paste the contents where you need
```
