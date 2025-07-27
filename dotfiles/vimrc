set nospell
set nocompatible
filetype indent plugin on
set wildmenu
set showcmd
set hlsearch
set ignorecase
set smartcase
set backspace=indent,eol,start
set autoindent
set nostartofline
set laststatus=2
set cmdheight=2
set shiftwidth=4
set softtabstop=4
set expandtab
set noshiftround
set showmode
set encoding=utf-8
set nobackup
set nowb
set noswapfile
set showmatch
set fileformat=unix

nnoremap <F3> :set invpaste paste?<CR>
set pastetoggle=<F3>


set statusline=                                                    " clear the statusline for when vimrc is reloaded
set statusline+=%-3.3n\                                            " buffer number
set statusline+=%f\                                                " file name
set statusline+=%h%m%r%w                                           " flags
set statusline+=[%{strlen(&ft)?&ft:'none'},                        " filetype
set statusline+=%{strlen(&fenc)?&fenc:&enc},                       " encoding
set statusline+=%{&fileformat}]                                    " file format
set statusline+=%=                                                 " right align
set statusline+=%{synIDattr(synID(line('.'),col('.'),1),'name')}\  " highlight
set statusline+=%b,0x%-8B\                                         " current char
set statusline+=%-14.(%l,%c%V%)\ %<%P                              " offset

autocmd BufWritePre * :%s/\s\+$//e
autocmd BufRead,BufNewFile *.yaml,*.yml set filetype=yaml
autocmd BufRead,BufNewFile *.j2 set filetype=jinja
autocmd FileType yaml setlocal ts=2 sts=2 sw=2 expandtab

