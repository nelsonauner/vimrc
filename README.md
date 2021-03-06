# setup

## OSX / \*nix

```shell
sudo apt-get install vim -y
sudo apt-get install git -y 
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
git clone https://github.com/nelsonauner/vim.git ~/vim
cp ~/vim/_vimrc ~/.vimrc
vi ~/.vimrc
:so %
:PluginInstall
```

## Windows 

```shell
choco install vim
choco install git
```

(or install them some other way)
then, with git bash:
```shell
cd ~
git clone https://github.com/gmarik/Vundle.vim.git ~/vimfiles/bundle/Vundle.vim
git clone -b windows https://github.com/nelsonauner/vim.git ~/vim
cp ~/vim/_vimrc ~/.vimrc
gvim .vimrc
:so %
:PluginInstall
```


# Troubleshooting

Try these to understand where vim is looking for your config files
```shell
:e $MYVIMRC
:help runtimepath
```

```shell
:version
:echo expand('~')
:echo $HOME
:echo $VIM
:echo $VIMRUNTIME
