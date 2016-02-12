# Simple .vimrc config

```
set expandtab
set tabstop=4
syntax on
set softtabstop=4
set shiftwidth=4
set autoindent
set hlsearch

autocmd BufRead,BufNewFile Makefile set noexpandtab

" For tex files set a line lenght limit to maximum of 80 characters
au BufRead,BufNewFile *.tex set tw=8
```
