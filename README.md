# MACBOOK SETUP

- [ ] INSTALL ROSETTA2 `/usr/sbin/softwareupdate --install-rosetta --agree-to-license`
- [ ] INSTALL HOMEBREW `- /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- [ ] DOWNLOAD THE [SETUP-MAC](https://github.com/gianpozzobon/setup-mac) REPOSITORY AND UNZIP
- [ ] ENTER IN THE REPOSITORY DIRECTORY
- [ ] RUN `chmod +x brew-installs.sh`
- [ ] RUN _brew-install_ SCRIPT `- ./brew-installs.sh`
- [ ] COPY iTerm2 AND CONFIGURE TO OPEN WITH ROSETTA2
- [ ] RUN `echo $SHELL`. IF OUTPUT NOT IS `/bin/zsh` RUN `chsh -s $(which zsh)`
- [ ] INSTALL OH MY ZSH `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- [ ] ENTER IN ZSH DIRECTORY TO INSTALL PLUGINS `cd $HOME/.oh-my-zsh/plugins`
- [ ] CLONE PLUGIN `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git`
- [ ] APPEND IN .zshrc FILE `echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc`
- [ ] INSERT THE CODE IN `.zshrc`

```
export NVM_DIR="$HOME/.nvm"
#This loads nvm
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
#This loads nvm bash_completion
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
```

- [ ] SETUP GITHUB

```
git config --global user.name "Gian Pozzobon" &&
git config --global user.email gian@plincondominios.com.br &&
git config --global --list
```

- [ ] INSTALL POWERLINE FONTS

```SH
git clone https://github.com/powerline/fonts.git --depth=1 &&
cd fonts &&
./install.sh &&
cd ..
```
