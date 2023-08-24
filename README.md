To fork
1. create new repo
2. clone new repo
3. add this as upstream, e.g.
  `git remote  add upstream git@github.com:guymatz/latex-base.git`
4. pull code to new repo, e.g.
  `git pull upstream main`
5. push to new repo, e.g.
  `git push origin main`

Ensure the following are set in .vimrc
" snippets
let g:UltiSnipsExpandTrigger = '<tab>'
let g:UltiSnipsJumpForwardTrigger = '<tab>'
let g:UltiSnipsJumpBackwardTrigger = '<s-tab>'
let g:UltiSnipsEditSplit="vertical"
let g:UltiSnipsSnippetDirectories=[".tex", "UltiSnips"]
"set runtimepath+=.tex

" vim-snipmate
set runtimepath^=./.tex

"let g:snipMate.snippet_dirs = [".tex"]

" vimtex
let g:vimtex_compiler_method = "latexrun"
let g:tex_flavor='latex'
let g:vimtex_view_method='skim'
"let g:vimtex_view_method='zathura'
let g:vimtex_quickfix_mode=0
let g:vimtex_fold_enabled=1
let g:vimtex_format_enabled=1

" KeitaNakamura/tex-conceal.vim
set conceallevel=1
let g:tex_conceal='abdmg'
hi Conceal ctermbg=none

