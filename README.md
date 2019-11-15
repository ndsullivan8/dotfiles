# Dotfiles
TO INSTALL
```
git clone https://github.com/ndsullivan8/dotfiles.git
```
## Vim SETUP
```
cd ~/dotfiles/vim/
python bootstrap.py
cd ~
ln -fs ~/dotfiles/vim/vimrc ~/.vimrc
```

## YouCompleteMe SETUP
```
cd ~/dotfiles/vim/bundle
git clone https://github.com/ycm-core/YouCompleteMe.git
git submodule update --init --recursive
cd YouCompleteMe
git submodule update --init --recursive
./install.py --clang-completer --go-completer
```

## Final
```
ln -fs ~/dotfiles/vim/vimrc ~/.vimrc
ln -fs ~/dotfiles/tmux.conf ~/.tmux.conf
```
