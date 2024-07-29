# NVIM
- to downlaod nvim

```
apt install nvim
```

- Create .config/nvim/init.vim
- OR Create ~/.vimrc
 
```
set number
set hlsearch
set mouse=a
syntax on
set cursorline 
:highligh Cursorline cterm=bold ctermbg=black

set ignorecase 
set smartcase

set tabstop =4
set softtabstop =4
set shiftwidth =4
set textwidth =79
set expandtab
set autoindent

set showmatch

if !has('gui_running')
    set t_Co=256
endif
```
