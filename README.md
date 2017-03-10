# vim-settings
My Vim settings

## Plugins used
  * NERDTree
  * Pathogen
  * CtrlP
  * Powerline
  
  
```
execute pathogen#infect()                                                   
colorscheme molokai        
syntax on                  
filetype plugin indent on
au BufNewFile,BufRead *.ejs set filetype=html
set runtimepath^=~/.vim/bundle/ctrlp.vim
set rtp+=/user/local/lib/python2.7/dist-packages/powerline/bindings/vim/
let g:EditorConfig_exclude_patterns = ['fugitive://.*']

let g:NERDTreeChDirMode = 2
set shiftwidth=2           
set tabstop=2              
set expandtab              

let g:ctrlp_max_files=0    
let g:ctrlp_max_depth=40   
let g:ctrlp_working_path_mode = 'rw'
let g:ctrlp_custom_ignore = {
  \ 'dir': '\v[\/](\.git|node_modules|\.sass-cache|bower_components|build)$',
  \ 'file': '\v\.(exe|so|dll)$',
  \ 'link': 'some_bad_symbolic_links',
  \ }

autocmd vimenter * NERDTree

au BufLeave * :wa
au FocusLost * :wa

" Set line number
set number

set showcmd " show command in bottom bar

set cursorline

set wildmenu

set lazyredraw

set showmatch

set incsearch
set hlsearch

filetype indent otn
```
