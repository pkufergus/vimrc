Best vimrc for CoolCeph team, used for C/C++, Python, PHP and Go.

The design principles of coolceph vimrc is simple, green and easy. Coolceph vimrc is designed running well on Linux and Mac, just need ctags, git and powerline_fonts. And also coolceph vimrc can be copied and installed anywhere by just a tarball.

Enjoy it.

![alt tag](https://raw.github.com/coolceph/vimrc/master/screenshot-2.png)

# Install

* vimrc will install to ~/.vim, require ~/.vim does not exist.

```
bash -c "$( curl https://raw.githubusercontent.com/coolceph/vimrc/master/setup.sh )"
```

# ShortCuts

| Key            | Function                                            |
| -------------- | --------------------------------------------------- |
| F2             | Paste mode toggle(normal/paste)                     |
| F3             | NerdTREE toggle                                     |
| F4             | Tagbar toggle                                       |
| F5             | LineNumber Model Switch                             |
| F6             | Whether or not show listchar                        |
| F7             | Update ctags                                        |
| F8             | Open undotree                                       |
| F9             | Enter multi-cursor-mode                             |
| F12            | Mouse mode switch (mouse=a/-a)                      |
| SpaceSpace     | Activate Unite Search Plugin                        |
| Ctrl+n/p       | Switch between buffers.                             |
| Ctrl+h/j/k/l   | Switch between windows.                             |
| Ctrl+c         | Completely quit vim without saving                  |

The leader key is ','.

# Quick Commands

| Cmd     | Function                   |
| ------- | -------------------------- |
| Ctags   | Genrate ctags for pwd      |
| Gotags  | Genrate gotags for pwd     |
| Hex/Asc | Swtich between Asc and Hex |
| Cswp    | Clear swp files            |

# FAQ

- *How should I install vimrc on a Linux server with no internet*

    Vim version 7.4+ is needed on your Linux server, then the steps:

    1) You need install vimrc on a Mac/Linux with internet first.

    2) Then run "~/.vim/setup.sh -b", a "vimrc-2016xxxx-mini.tar.gz" file will appear in your ~ dir.

    3) Copy the "vimrc-2016xxxx-mini.tar.gz" to your user's home dir on Linux server.

    4) Run "cd ~;rm -rf ~/.vim;tar -zxvf vimrc-2016xxxx-mini.tar.gz;.vim/setup.sh -l"

    You now get full-featured vimrc on your Linux server.

- *My state line has strange characters*

    You should install the powerline fonts into your system and update the config of your terminal to use powerline fonts to display the Non-ASCII characters.

    In the fonts dir, there is some powerline fonts you could choose.

    You could found more powerline fonts in [powerline_fonts]

- *My vim is ugly, it seems some color are missing*

    You should set your env TERM=xterm-256color, you can do this by the following two ways:

    1) run ~/.vim/install.sh, it will set TERM to xterm-256color for bash/zsh. If you use other shells, you need to set TERM yourself.

    2) Your terminal util like iterm is also needed to set for xterm-256color too. You need set it yourself too.

# Plugins used in CoolCeph vimrc

[STL-Syntax]

[ack.vim]

[ag.vim]

[csv.vim]

[jellybeans.vim]

[neocomplcache.vim]

[neomru.vim]

[neosnippet-snippets]

[neosnippet.vim]

[nerdcommenter]

[nerdtree]

[papercolor-theme]

[rainbow_parentheses.vim]

[tabular]

[tagbar]

[tagbar-phpctags.vim]

[taghighlight]

[undotree]

[unite.vim]

[vim-airline]

[vim-airline-themes]

[vim-colors-solarized]

[vim-easymotion]

[vim-fugitive]

[vim-gitgutter]

[vim-go]

[vim-indexed-search]

[vim-multiple-cursors]

[vim-pathogen]

[vim-signature]

[vim-togglenumber]

[vimproc.vim]

[vimshell.vim]

[vim-expand-region]

[vim-trailing-whitespace]

[vim-surround]

[vim-repeat]

[a.vim]

[indentLine]

[STL-Syntax]:https://github.com/Mizuchi/STL-Syntax
[ack.vim]:https://github.com/mileszs/ack.vim
[ag.vim]:https://github.com/rking/ag.vim
[csv.vim]:https://github.com/chrisbra/csv.vim
[jellybeans.vim]:https://github.com/nanotech/jellybeans.vim
[neocomplcache.vim]:https://github.com/Shougo/neocomplcache.vim
[neomru.vim]:https://github.com/Shougo/neomru.vim
[neosnippet-snippets]:https://github.com/Shougo/neosnippet-snippets
[neosnippet.vim]:https://github.com/Shougo/neosnippet.vim
[nerdcommenter]:https://github.com/scrooloose/nerdcommenter
[nerdtree]:https://github.com/scrooloose/nerdtree
[papercolor-theme]:https://github.com/NLKNguyen/papercolor-theme
[rainbow_parentheses.vim]:https://github.com/kien/rainbow_parentheses.vim
[tabular]:https://github.com/godlygeek/tabular
[tagbar]:https://github.com/majutsushi/tagbar
[tagbar-phpctags.vim]:https://github.com/vim-php/tagbar-phpctags.vim
[taghighlight]:https://github.com/abudden/taghighlight-automirror
[undotree]:https://github.com/mbbill/undotree
[unite.vim]:https://github.com/Shougo/unite.vim
[vim-airline]:https://github.com/bling/vim-airline
[vim-airline-themes]:https://github.com/vim-airline/vim-airline-themes
[vim-colors-solarized]:https://github.com/altercation/vim-colors-solarized
[vim-easymotion]:https://github.com/easymotion/vim-easymotion
[vim-fugitive]:https://github.com/tpope/vim-fugitive
[vim-gitgutter]:https://github.com/airblade/vim-gitgutter
[vim-go]:https://github.com/fatih/vim-go
[vim-indexed-search]:https://github.com/henrik/vim-indexed-search
[vim-multiple-cursors]:https://github.com/terryma/vim-multiple-cursors
[vim-pathogen]:https://github.com/tpope/vim-pathogen
[vim-signature]:https://github.com/kshenoy/vim-signature
[vim-togglenumber]:https://github.com/tkhoa2711/vim-togglenumber
[vimproc.vim]:https://github.com/Shougo/vimproc.vim.git
[vimshell.vim]:https://github.com/Shougo/vimshell.vim
[vim-expand-region]://github.com/terryma/vim-expand-region
[vim-trailing-whitespace]:https://github.com/bronson/vim-trailing-whitespace
[vim-surround]:https://github.com/tpope/vim-surround
[vim-repeat]://github.com/tpope/vim-repeat
[a.vim]:https://github.com/vim-scripts/a.vim
[indentLine]:https://github.com/Yggdroot/indentLine
[powerline_fonts]:https://github.com/powerline/fonts

