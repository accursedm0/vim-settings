set bg=dark
set modelines=5
set incsearch
set tabstop=2
set shiftwidth=2
set expandtab
set undolevels=20
syntax on
map Q gq
let spell_executable = "aspell"
let spell_language_lsist = 'english'
let spell_insert_mode = 0
filetype on
filetype plugin on
filetype indent on
set t_Co=256
set pastetoggle=<F2>
nnoremap <silent> <F8> :TlistToggle<CR>
let Tlist_GainFocus_On_ToggleOpen = 1
let Tlist_Exit_OnlyWindow = 1
let Tlist_Close_On_Select = 1
let Tlist_Sort_Type = "name"
set number
set cursorline
set cursorcolumn
colorscheme mustang
"colorscheme solarized
"colorscheme codeschool

" careful, this breaks special chars in  latin encoded files cause vim opens
" it as utf-8 for good
if has("multi_byte")
  if &termencoding == ""
    let &termencoding = &encoding
  endif
  set encoding=utf-8
  setglobal fileencoding=utf-8
  "setglobal bomb
  set fileencodings=utf-8,latin1
endif

augroup resCur
  autocmd!
  autocmd BufReadPost * call setpos(".", getpos("'\""))
augroup END

set dictionary+=/usr/share/dict/words

set laststatus=2

let g:airline_powerline_fonts = 1
let g:airline_theme='powerlineish'

if !exists('g:airline_symbols')
  let g:airline_symbols = {}
endif
let g:airline_symbols.space = "\ua0"

" set statusline=%{fugitive#statusline()}
