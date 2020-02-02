# Termux Coding

1. Install package
```bash
$ pkg update && pkg upgrade && pkg install git vim procps proot​ nodejs-lts python golang build-essential cmake patch curl
```
2. Restart termux
3. Setup proot
```bash
$ cd ~ && curl -fsSL https://raw.githubusercontent.com/theimpostor/termux-vim-ycm/master/bashrc.patch | patch
```
4. Restart termux
5. Install vundle
```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
5. Setup .vimrc w/vundle, ycm, vim-go
```bash
curl -fsSL https://raw.githubusercontent.com/theimpostor/termux-vim-ycm/master/vundle.vimrc >> ~/.vimrc
```
6. Vim install plugins
```bash
vim +PluginInstall +qall
```
7. Build ycm binary
```bash
cd ~/.vim/bundle/YouCompleteMe && ./install.py --go-completer --clang-completer --system-libclang
```
