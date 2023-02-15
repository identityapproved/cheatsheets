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

  
## How to undo a local commit

Let's say I committed locally, but now I want to remove that commit.

```
git log
    commit 101: bad commit    # Latest commit. This would be called 'HEAD'.
    commit 100: good commit   # Second to last commit. This is the one we want.
```

To restore everything back to the way it was prior to the last commit, we need to `reset` to the commit before `HEAD`:

```
git reset --soft HEAD^     # Use --soft if you want to keep your changes
git reset --hard HEAD^     # Use --hard if you don't care about keeping the changes you made
```

Now `git log` will show that our last commit has been removed.

## How to undo a public commit

If you have already made your commits public, you will want to create a new commit which will "revert" the changes you made in your previous commit (current HEAD).

```
git revert HEAD
```

Your changes will now be reverted and ready for you to commit:

```
git commit -m 'restoring the file I removed by accident'
git log
    commit 102: restoring the file I removed by accident
    commit 101: removing a file we don't need
    commit 100: adding a file that we need
```

For more information, check out _[Git Basics - Undoing Things](https://git-scm.com/book/en/v2/Git-Basics-Undoing-Things)_.