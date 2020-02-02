# Termux Coding

1. Install package
```bash
$ pkg update && pkg upgrade && pkg install git vim procps proot​ nodejs-lts python golang build-essential cmake patch curl
```
2. Restart Termux
3. Setup proot
```bash
$ cd ~ && curl -fsSL https://raw.githubusercontent.com/theimpostor/termux-vim-ycm/master/bashrc.patch | patch
```
