---
Tags: #linux/terminal #linux/terminal #terminal/tools #terminal/tools/nvm 
Medium: #terminal #linux 
---
Tags: #linux/terminal #linux/terminal #terminal/tools #terminal/tools/nvm 
Medium: #terminal #linux 
Links:
___

### Install & Update Script

To **install** or **update** nvm, you should run the [install script](https://github.com/nvm-sh/nvm/blob/v0.39.3/install.sh). To do that, you may either download and run the script manually, or use the following cURL or Wget command:
```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
```shell
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

Running either of the above commands downloads a script and runs it. The script clones the nvm repository to `~/.nvm`, and attempts to add the source lines from the snippet below to the correct profile file (`~/.bash_profile`, `~/.zshrc`, `~/.profile`, or `~/.bashrc`).
```shell
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```

[NVM GitHub](https://github.com/nvm-sh/nvm#additional-notes)

Install node+npm:
```shell
nvm install node # Install the latest available version  
nvm install --lts # Install the latest LTS version  
```