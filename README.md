# Dotfiles
TO INSTALL
```
git clone https://github.com/ndsullivan8/dotfiles.git
```

## Oh-My-Zsh

```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## HomeBrew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)
```

## Mac OS
```
brew install python
brew install vim
export PATH=/usr/local/bin:/usr/local/sbin:$PATH
```

## Vim Pkgs
```
cd ~/dotfiles/vim/
pip3 install --user requests
python3 bootstrap.py
cd ~
ln -fs ~/dotfiles/vim/vimrc ~/.vimrc
```

## YouCompleteMe
```
cd ~/dotfiles/vim/bundle
git clone https://github.com/ycm-core/YouCompleteMe.git
cd YouCompleteMe
git submodule update --init --recursive
./install.py --clang-completer --go-completer
```

## Final
```
rm -f ~/.zshrc
ln -fs ~/dotfiles/zshrc ~/.zshrc
ln -fs ~/dotfiles/tmux.conf ~/.tmux.conf
ln -fs ~/dotfiles/vim/vimrc ~/.vimrc
```
